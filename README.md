@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400&display=swap');

/** Variables - colors **/
:root {
    /* Light */
    --color-light-50: black;

    /* Dark */
    --color-dark-50: #e7b018;
    --color-dark-100: #e7b018;
    --color-dark-900: #e7b018;

    /* Purple */
    --color-purple-50: #ffffff;
    --color-purple-100: #ffffff;
    --color-purple-200:#ffffff;

    /* Gradient */
    --color-gradient: linear-gradient(90deg, var(--color-purple-50), var(--color-purple-100), var(--color-purple-200));
}

/* General */
* {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header{
    background-color: black;
    width: 100%;
    padding: 15px 4%;
    position: sticky;
    top: 0;
    z-index: 9999;
}

.container1{
    max-width: 1080px;
    margin: 0 auto;
    display: flex;
    align-items: center;
}



.content{
    align-items: center;
    justify-content: space-around;
    padding: 0 3%;

}
.logo{
    width: 25%;
}

.logo img{
    width: 55px;
    cursor: pointer;
}

.menu{
width: 75%;
}

.menu nav a{
color: #c4c4c4;
text-decoration: none;
font-size: 18px;
padding-right: 30px;
padding-bottom: 8px;
position: relative;
justify-content: space-between;
}

.menu nav a::after{
content: " ";
width: 0px;
height: 4px;
background-image: linear-gradient(45deg , #eeff00, #FF7100);
position: absolute;
bottom: 0;
left: 0;
transition: width 0.5s;
}

.menu nav a:hover::after{
width: 30px;
}


#container {
    height: 100vh;
    width: 100%;
    display: flex;
    background: var(--color-gradient);
    justify-content: center;
    align-items: center;
}

#login_form {
    display: flex;
    flex-direction: column;
    height: fit-content;
    background-color: var(--color-light-50);
    padding: 30px 40px;
    border-radius: 8px;
    gap: 30px;
    box-shadow: 5px 5px 8px rgba(0, 0, 0, 0.336);
    animation: dark-to-light-background 0.3s ease-in-out;
}

#login_form h2 {
    font-size: 24px;
    text-align: center;
    margin-bottom: 20px;
    color: #e7b018;
}

#inputs {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 20px;
}

.input-box label {
    font-size: 14px;
    color: var(--color-dark-50);
}

.input-field {
    display: flex;
    align-items: center;
    gap: 15px;
    padding: 3px;
    border-bottom: 1px solid var(--color-purple-50);
    cursor: text;
}

.input-field i {
    font-size: 18px;
    cursor: text;
    color: var(--color-dark-900);
} 

.input-field input {
    border: none;
    width: 260px;
    background-color: transparent;
    font-size: 18px;
    padding: 0px 5px;
}

.input-field input:focus {
    outline: none;
}

#login_button {
    border: none;
    background: var(--color-gradient);
    padding: 7px;
    border-radius: 3px;
    color: var(--color-light-50);
    font-weight: bold;
    font-size: 18px;
    cursor: pointer;
}

#login_button:hover {
    transform: scale(1.05);
}
