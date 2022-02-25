<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><span class="red">{</span><span id="brand">rev</span><span class="red">}</span></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor02" aria-controls="navbarColor02" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarColor02">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">SIGN UP
                            <span class="visually-hidden">(current)</span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">SIGN IN</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">Dropdown</a>
                        <div class="dropdown-menu">
                            <a class="dropdown-item" href="#">Action</a>
                            <a class="dropdown-item" href="#">Another action</a>
                            <a class="dropdown-item" href="#">Something else here</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Separated link</a>
                        </div>
                    </li>
                </ul>
                <form class="d-flex">
                    <input class="form-control me-sm-2" type="text" placeholder="Search">
                    <button class="btn-sm btn-secondary" type="submit"><i class="fas fa-search"></i></button>
                </form>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    li {
        background-color: rgba(0, 0, 0, 0.308);
        padding: 0.5rem;
    }

    nav {
        -webkit-box-shadow: 0px 8px 50px 5px rgba(0,0,0,0.64); 
        box-shadow: 0px 8px 50px 5px rgba(0,0,0,0.64);
        z-index: 2;
        position: sticky;
        top: 0;
    }

    .navbar-brand {
        font-family: 'Bebas Neue', cursive;
        font-size: 2.8125rem;
        height: 4.5rem;
        text-align: center;
        transition: 0.4s;
    }

    .navbar-brand:hover #brand {
        color: #BC3323;
    }

    .navbar-brand span{
        transition: 0.4s;
    }

    .navbar-brand:hover span {
        color: white;
    }

    .container-fluid {
        height: 2.5rem;
    }

    input {
        transition: 0.4s;
        width: 12.5rem;
        background-color: rgba(255, 255, 255, 0.336);
        color: black;
    }

    input:focus {
        border: #BC3323 solid 0.0313rem;
        border-radius: 0.1875rem;
        width: 15.625rem;
    }

    button {
        background-color: #BC3323;
        font-family: 'Bebas Neue', cursive; 
        font-size: 1.25rem;
        width: 3.125rem;
        transition: 0.4s;
    }

    button:active, button:hover, button:focus {
        color: #BC3323;
        background-color: white;
        border-radius: 0.1875rem
    }

    .nav-item {
        border-radius: 0.6rem;
        margin-left: 0.1875rem;
        padding-bottom: 2.8125rem;
        height: 2.9375rem;
    }

    a {
        transition: 0.4s;
    }

    .dropdown-item:active {
            background-color: #BC3323;
    }

    @media only screen and (max-width: 992px) {
        nav {
            
        }

        .navbar-toggler {
            position: absolute;
            top: 15px;
            right: 10px;
        }

        .navbar-brand {
            position: absolute;
            top: 0;
            left: 10px;
        }

        input {
            display: block;
            margin: 0 auto 0 0;
            width: 100%;
        }

        .nav-item {
            margin: 0 0 5px 0;
        }

        .btn-sm {
            width: 20%;
            margin-left: 5px;
        }
        
        input:focus {
            width: 100%;
        }

        .navbar-collapse {
            padding: 55px 10px 10px 10px;
            margin: 0;
            background-color: #212529;
            border-radius: 10px;
        }
    }
</style>