<!DOCTYPE html>
<html lang="en">
<head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css" integrity="sha512-HK5fgLBL+xu6dm/Ii3z4xhlSUyZgTT9tuc/hSrtw6uzJOvgRr2a9jyxxT1ely+B+xFAmJKVSTbpM/CuL7qxO8w==" crossorigin="anonymous" />
</head>
<body>

    <div class="container">

        <div class="row pt-4 pb-4">
            <div class="col-4 text-center">
            </div>

            <div class="col-4 text-center">
                <select class="custom-select">

                    <option value="2">Feb 2021</option>
                    <option value="e">Jan 2021</option>
                </select>
            </div>
            <div class="col-4 text-center">
            </div>
        </div>

        <div id="accordion">

            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingOne">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-01-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">PAM Listed</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                01-10-2021
                                <a href="#" class="text-secondary">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>

                <div id="collapseOne" class="collapse " aria-labelledby="headingOne" data-parent="#accordion">
                    <div class="card-body">
                        <div class="card-body">
                            <table class="table table-striped">
                                <thead>
                                    <tr>
                                        <th scope="col">#</th>
                                        <th scope="col">First</th>
                                        <th scope="col">Last</th>
                                        <th scope="col">Handle</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <th scope="row">1</th>
                                        <td>Mark</td>
                                        <td>Otto</td>
                                        <td>@mdo</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">2</th>
                                        <td>Jacob</td>
                                        <td>Thornton</td>
                                        <td>@fat</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">3</th>
                                        <td>Larry</td>
                                        <td>the Bird</td>
                                        <td>@twitter</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </div>
            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingTwo">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-08-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">PAM Unlisted</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                01-11-2021
                                <a href="#" class="text-secondary">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseTwo" aria-expanded="true" aria-controls="collapseTwo">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>
                <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#accordion">
                    <div class="card-body">
                        <div class="card-body">
                            <table class="table table-striped">
                                <thead>
                                    <tr>
                                        <th scope="col">#</th>
                                        <th scope="col">First</th>
                                        <th scope="col">Last</th>
                                        <th scope="col">Handle</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <th scope="row">1</th>
                                        <td>Mark</td>
                                        <td>Otto</td>
                                        <td>@mdo</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">2</th>
                                        <td>Jacob</td>
                                        <td>Thornton</td>
                                        <td>@fat</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">3</th>
                                        <td>Larry</td>
                                        <td>the Bird</td>
                                        <td>@twitter</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </div>

            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingThree">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-15-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">LMS Unlisted</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                01-15-2021
                                <a href="#" class="text-secondary">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseThree" aria-expanded="true" aria-controls="collapseThree">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>
                <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#accordion">
                    <div class="card-body">
                        <div class="card-body">
                            <table class="table table-striped">
                                <thead>
                                    <tr>
                                        <th scope="col">#</th>
                                        <th scope="col">First</th>
                                        <th scope="col">Last</th>
                                        <th scope="col">Handle</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <th scope="row">1</th>
                                        <td>Mark</td>
                                        <td>Otto</td>
                                        <td>@mdo</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">2</th>
                                        <td>Jacob</td>
                                        <td>Thornton</td>
                                        <td>@fat</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">3</th>
                                        <td>Larry</td>
                                        <td>the Bird</td>
                                        <td>@twitter</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </div>

            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingFour">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-24-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">RML Unlisted</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                01-16-2021
                                <a href="#" class="text-secondary">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseFour" aria-expanded="true" aria-controls="collapseFour">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>
                <div id="collapseFour" class="collapse" aria-labelledby="headingFour" data-parent="#accordion">
                    <div class="card-body">
                        <div class="card-body">
                            <table class="table table-striped">
                                <thead>
                                    <tr>
                                        <th scope="col">#</th>
                                        <th scope="col">First</th>
                                        <th scope="col">Last</th>
                                        <th scope="col">Handle</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <th scope="row">1</th>
                                        <td>Mark</td>
                                        <td>Otto</td>
                                        <td>@mdo</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">2</th>
                                        <td>Jacob</td>
                                        <td>Thornton</td>
                                        <td>@fat</td>
                                    </tr>
                                    <tr>
                                        <th scope="row">3</th>
                                        <td>Larry</td>
                                        <td>the Bird</td>
                                        <td>@twitter</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </div>

            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingFive">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-25-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">RML Unlisted</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                01-17-2021
                                <a href="#" class="text-primary" type="button" data-toggle="modal" data-target="#exampleModal">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseFive" aria-expanded="true" aria-controls="collapseFive">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>
                <div id="collapseFive" class="collapse" aria-labelledby="headingFive" data-parent="#accordion">
                </div>
            </div>

            <div class="card">
                <div class="card-header d-flex justify-content-start" id="headingFive">

                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Date Of Month</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">02-26-2021</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0 pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Transaction Type</p>
                        </div>
                        <div class="bd-highlight">
                            <p class="h5">RML Unlisted</p>
                        </div>
                    </div>
                    <div class="d-flex flex-column bd-highlight mb-0  pr-4">
                        <div class="bd-highlight">
                            <p class="h6">Validity Date</p>
                        </div>
                        <div class="bd-highlight d-flex flex-row ">
                            <p class="h5 ">
                                Nil
                                <a href="#" class="text-primary" type="button" data-toggle="modal" data-target="#exampleModal">
                                    <i class="pl-2 fas fa-edit"></i>
                                </a>
                            </p>
                        </div>
                    </div>

                    <button class="btn btn-link ml-auto " data-toggle="collapse" data-target="#collapseFive" aria-expanded="true" aria-controls="collapseFive">
                        <i class="fas fa-chevron-down"></i>
                    </button>
                </div>
                <div id="collapseFive" class="collapse" aria-labelledby="headingFive" data-parent="#accordion">
                </div>
            </div>
        </div>
    </div>
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLabel">Select validity date for 02-25-2021</h5>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">&times;</span>
                    </button>
                </div>
                <div class="modal-body">
                    <input type="date" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
                    <p>  </p>
                    <p> OR </p>

                    <select class="custom-select">

                        <option value="1">01-02-2021</option>
                        <option value="2">01-03-2021</option>
                        <option value="2">01-04-2021</option>
                        <option value="3">01-05-2021</option>
                    </select>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
                    <button type="button" class="btn btn-primary">Save changes</button>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
