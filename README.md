 var server = new Server(@".");
            var databse = server.Databases["InfinityMatrix.Niraiya"];
            string path = @"C:\Work\DB\" + databse.Name + @"\";

            var scripter = new Scripter(server);
            scripter.Options.ScriptDrops = false;
            scripter.Options.WithDependencies = false;
            scripter.Options.IncludeHeaders = false;
            scripter.Options.Indexes = true;
            scripter.Options.Triggers = true;

            var smoObjects = new Urn[1];
            foreach (Table t in databse.Tables)
            {
                smoObjects[0] = t.Urn;
                if (t.IsSystemObject == false)
                {
                    StringCollection sc = scripter.Script(smoObjects);

                    var sb = new StringBuilder();

                    foreach (var st in sc)
                    {
                        sb.AppendLine(st);
                        sb.AppendLine("GO");
                        sb.AppendLine("");
                    }

                    bool exists = System.IO.Directory.Exists(path + "Tables");

                    if (!exists)
                        System.IO.Directory.CreateDirectory(path + "Tables");

                    using (System.IO.StreamWriter file = new System.IO.StreamWriter(path + @"Tables\" + t.Name + ".sql"))
                    {
                        file.WriteLine(sb.ToString()); // "sb" is the StringBuilder
                    }
                }
            }

            foreach (StoredProcedure t in databse.StoredProcedures)
            {
                if (t.IsSystemObject == false)
                {
                    smoObjects[0] = t.Urn;
                    StringCollection sc = scripter.Script(smoObjects);

                    var sb = new StringBuilder();

                    foreach (var st in sc)
                    {
                        sb.AppendLine(st);
                        sb.AppendLine("GO");
                        sb.AppendLine("");
                    }

                    bool exists = System.IO.Directory.Exists(path + "StoredProcedure");

                    if (!exists)
                        System.IO.Directory.CreateDirectory(path + "StoredProcedure");

                    using (System.IO.StreamWriter file = new System.IO.StreamWriter(path + @"StoredProcedure\" + t.Name + ".sql"))
                    {
                        file.WriteLine(sb.ToString()); // "sb" is the StringBuilder
                    }
                }
            }

            foreach (UserDefinedFunction t in databse.UserDefinedFunctions)
            {
                if (t.IsSystemObject == false)
                {
                    smoObjects[0] = t.Urn;

                    StringCollection sc = scripter.Script(smoObjects);

                    var sb = new StringBuilder();

                    foreach (var st in sc)
                    {
                        sb.AppendLine(st);
                        sb.AppendLine("GO");
                        sb.AppendLine("");
                    }

                    bool exists = System.IO.Directory.Exists(path + "UserDefinedFunction");

                    if (!exists)
                        System.IO.Directory.CreateDirectory(path + "UserDefinedFunction");

                    using (System.IO.StreamWriter file = new System.IO.StreamWriter(path + @"UserDefinedFunction\" + t.Name + ".sql"))
                    {
                        file.WriteLine(sb.ToString()); // "sb" is the StringBuilder
                    }
                }
            }

            foreach (UserDefinedDataType t in databse.UserDefinedDataTypes)
            {
                smoObjects[0] = t.Urn;
                if (true == true)
                {
                    StringCollection sc = scripter.Script(smoObjects);

                    var sb = new StringBuilder();

                    foreach (var st in sc)
                    {
                        sb.AppendLine(st);
                        sb.AppendLine("GO");
                        sb.AppendLine("");
                    }

                    bool exists = System.IO.Directory.Exists(path + "UserDefinedDataType");

                    if (!exists)
                        System.IO.Directory.CreateDirectory(path + "UserDefinedDataType");

                    using (System.IO.StreamWriter file = new System.IO.StreamWriter(path + @"UserDefinedDataType\" + t.Name + ".sql"))
                    {
                        file.WriteLine(sb.ToString()); // "sb" is the StringBuilder
                    }
                }
            }

            Console.ReadLine();
