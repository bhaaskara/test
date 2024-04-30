<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Horizontal Navigation with Dropdown</title>
  <style>
    /* Style the navigation bar */
    .navigation {
      background-color: #333;
      color: #fff;
      display: flex;
      justify-content: space-between;
      padding: 10px 20px;
    }

    .navigation a {
      color: inherit;
      text-decoration: none;
      padding: 10px 15px;
    }

    .navigation a:hover {
      background-color: #222;
    }

    /* Style the dropdown list */
    .dropdown {
      position: relative;
      display: inline-block;
    }

    .dropdown-content {
      display: none;
      position: absolute;
      background-color: #f1f1f1;
      min-width: 160px;
      box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
      z-index: 1;
    }

    .dropdown-content a {
      color: black;
      padding: 12px 16px;
      text-decoration: none;
      display: block;
    }

    .dropdown-content a:hover {background-color: #ddd;}

    .dropdown:hover .dropdown-content {display: block;}
  </style>
</head>
<body>
  <header>
    <nav class="navigation">
      <a href="#">Home</a>
      <div class="dropdown">
        <a href="#">Products</a>
        <div class="dropdown-content">
          <a href="#">Category 1</a>
          <a href="#">Category 2</a>
          <div class="dropdown"> <a href="#">Subcategory 1.1</a>
            <div class="dropdown-content">
              <a href="#">Subcategory 1.1.1</a>
              <a href="#">Subcategory 1.1.2</a>
            </div>
          </div>
          <a href="#">Category 3</a>
        </div>
      </div>
      <a href="#">About Us</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  </body>
</html>

