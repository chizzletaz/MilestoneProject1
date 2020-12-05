goal: circle border around social media icons:
.list-inline-item {
    background-color: #6c757d;
    border: 1px solid black;
    border-radius: 50%;
    height: 40px;
    width: 40px;
    padding: 7px:
    text-align: center;
issue: the icons aren't centered: ![uncentered icons](assets/img/test/icon border 1.png)
trials: put text align after border-radius: ![uncentered icons](assets/img/test/icon border 2.png)
so horizontally centered.
for vertically centered: 

solution: .list-inline-item {
    background-color: #6c757d;
    border: 1px solid #fff;
    border-radius: 50%;
    text-align: center;
    height: 40px;
    width: 40px;
    padding: 7px;
}
---------------------
goal: position footer elements to the side till viewport sm. 
below sm position footer elements on top of each other.
.list-inline {
    float: right;
    padding: 50px;
}

.footer-signup{
    float: left;
    padding: 50px;
}
issue: the elements don't wrap nicely below viewport sm. 
trial: use float-sm-right/left and remove float from  (in style.css)
on inspecting the padding is too large below 760px.
trial: change padding (of list-inline and footer-signup) to 50px auto.
Padding auto is no valid value.
solution: use margin in stead of padding, so: margin: 50px auto.
----------------
