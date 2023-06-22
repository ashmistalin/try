# try

## Index.html:
```
*{
    margin: 0;
    padding: 0;
    font-family: 'Noto-serif',serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth ;
}
body{
    background: black;
    color: aliceblue;
}
#header{
    width:100%;
    height: 100vh;
    background-image: url(images/background13.png);
    background-size:cover;
    background-position: center;
}
.container{
    padding: 10px 50px;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo{
    width: 150px;
    height: 100px;
}
nav ul li{
    display:inline-block;
    list-style: none;
    margin-top: 1px;
    margin-left: 20px;
}
nav ul li a{
    color: white;
    text-decoration: none;
    font-size: 15px;
    position: relative;
}
nav ul li a::after{
content: ' ';
width: 0%;
height: 3px;
background: lightcoral;
position: absolute;
left: 0;
bottom: -6px;
transition: 0.5s;
}
nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 100px;
    font-size: 19px;
}
.header-text h1{
    font-size: 50px;
}
.header-text h1 span{
    color:lightcoral;
}






#about{
    padding: 50px 0px;
    color: white;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-column1{
    flex-basis: 35%;
}
.about-column1 img{
    border-radius: 15px;
}
.about-column2{
    flex-basis: 60%;
}
.subtitle{
font-size: 50px;
font-weight: 600;
color: lightcoral;
font-family: 'Poppins',sans-serif;
}
.about-column2 p{
    margin-top: 20px;
    font-size: 18px;
    font-family: 'Libre Baskerville', serif;
}

.tab{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size: 20px;
    font-weight: 400px;
    cursor: pointer;
    position: relative;

}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: lightcoral;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contents ul li{
    list-style: none;
    margin: 20px 0px;
}
.tab-contents ul li span{
color:lightcoral;
font-size: 16px;
}
.tab-contents{
    display: none;
}
.tab-contents.active-tab{
    display: block;
}







#services{
    padding: 30px 0;
}
.services-list{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.services-list div{
    background: #262626;
    padding: 30px;
    font-size: 14px;
    font-weight: 300px;
    border-radius: 20px;
    transition: background 0.5s, transform 0.5s;
}
.services-list div i{
    font-size: 40px;
    margin-bottom: 10px;
}
.services-list div h2{
    font-size: 25px;
    font-weight: 500;
    margin-bottom: 15px;
    color: lightcoral;
}
.services-list div p{
    font-family: 'Lato', sans-serif;
    font-size: 15px;
}
.services-list div a{
    text-decoration: none;
    color: aliceblue;
    font-size: 13px;
    margin-top: 20px;
    display: inline-block;
}
.services-list div a:hover{
    color:lightcoral;
}
.services-list div:hover{
    background: rgb(45, 33, 40);
    transform: translateY(-10px);
}
.services-list div h2:hover{
    color: white;
}





#mywork{
    padding: 50px 0;
}
h3{
    margin-top: 30px;
        font-size: 20px;
}
.worklist{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.work1{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.work1 img{
    width: 400px;
    height: 500px;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s;
}
.layer{
    width: 100%;
    height:0;
    background: linear-gradient(rgba(0,0,0,0.6),#ff004f);
    border-radius: 10px;
    position: absolute;
    left:0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 18px;
    transition: heigth 0.5s;
}
.layer h3{
    font-weight: 500px;
    margin-bottom: 20px;
}
.work1:hover img{
    transform: scale(1.1);
}
.work1:hover .layer{
    height: 100%;
}
.btn{
    display:block;
margin: 50px auto;
width: fit-content;
border: 1px solid #ff004f;
padding: 14px 50px;
border-radius: 6px;
text-decoration: none;
color: white;
transition: background 0.5s;
}
.btn:hover{
    background:#ff004f;
}



.cotactleft{
    flex-basis: 35%;

}
.contactleft p{
margin-top: 30px;

}
.contactleft p i{
    color: lightcoral;
    margin-right: 30px;
    font-size: 15px;
}
.contactright{
    flex-basis:60%;
}
.socialicons{
margin-top: 30px;
}
.socialicons a{
       text-decoration: none;
       font-size: 30px;
       margin-right: 15px;
       color: #abaaba;
       display: inline-block;
       transition: transform 0.5s;
}
.socialicons a:hover{
    color: lightcoral;
    transform: translateY(-5px);
}
.btn.btn2{
    display: inline-block;
    background: lightcoral;
}
.btn.btn2:hover{
    background-color: #ff004f;
}
.contactright form{
    width: 100%;

}
form input,form textarea{
    width:100%;
border:0 ;
outline: none;
background:#262626;
padding: 15px;
margin: 15px 0;
color: #fff;
font-size: 18px;
border-radius: 6px;
}
form .btn2{
    padding: 14px 60px;
    font-size: 18px;
    margin-top: 20px;
    cursor: pointer;
}
form .btn2:hover{
    background-color: #ff004f;
}
.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background:#262626;
    font-weight: 300px;
    margin-top: 40px;

}
.copyright i{
    color: rgb(122, 5, 5);
}
```
