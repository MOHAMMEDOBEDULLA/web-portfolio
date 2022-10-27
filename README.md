# web-portfolio
<!DOCTYPE html>
<html lang="en">
<head>

<style>

@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  outline: none;
  border: none;
  text-transform: capitalize;
  transition: all 0.2s linear;
}
html {
  font-size: 62.5%;
  overflow-x: hidden;
  scroll-behavior: smooth;
}
body {
  background: #f7f7f7;
  font-family: "Poppins", sans-serif;
}

*::selection {
  background: #2b3dda;
  color: #fff;
}

html {
  font-size: 62.5%;
  overflow-x: hidden;
}
html::-webkit-scrollbar {
  width: 0.8rem;
}
html::-webkit-scrollbar-track {
  background: rgb(235, 202, 245);
}
html::-webkit-scrollbar-thumb {
  background: #420177;
}

/* pre loader start */
.loader-container {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 10000;
  background: #e6eff1;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  width: 100%;
}
.loader-container.fade-out {
  top: -120%;
}
/* pre loader end */

/* navbar starts */
header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.7rem 10%;
  height: 6.5rem;
  background-color: #fff;
  box-shadow: 0 1px 4px rgba(146, 161, 176, 0.3);
}
section {
  min-height: 100vh;
  padding: 2rem 9%;
}
.heading {
  font-size: 3.5rem;
  color: rgb(32, 32, 32);
  font-weight: 800;
  text-align: center;
}
.heading span {
  color: rgb(115, 3, 167);
}
header .logo {
  font-size: 1.9rem;
  font-weight: 800;
  text-decoration: none;
  color: #0e2431;
}
header .logo i {
  font-size: 2.2rem;
}
header .logo:hover {
  color: #fc8c05;
}
header .navbar ul {
  list-style: none;
  display: flex;
  justify-content: center;
  align-items: center;
}
header .navbar li {
  margin-left: 2.5rem;
}
header .navbar ul li a {
  font-size: 1.57rem;
  color: #0e2431;
  font-weight: 600;
  text-decoration: none;
  letter-spacing: 0.04rem;
  transition: 0.2s;
}
header .navbar ul li a.active,
header .navbar ul li a:hover {
  color: #011aff;
  border-bottom: 0.2rem solid #011aff;
  padding: 0.5rem 0;
}
/* navbar ends */

/* hamburger icon starts*/
#menu {
  font-size: 3rem;
  cursor: pointer;
  color: rgb(24, 2, 63);
  display: none;
}
@media (max-width: 768px) {
  #menu {
    display: block;
  }
  header .navbar {
    position: fixed;
    top: 6.5rem;
    right: -120%;
    width: 75%;
    height: 100%;
    text-align: left;
    align-items: flex-start;
    background-color: #0e0f31;
  }
  header .navbar ul {
    flex-flow: column;
    padding: 1rem;
  }
  header .navbar ul li {
    text-align: center;
    width: 100%;
    margin: 1rem 0;
    border-radius: 0.5rem;
    width: 26rem;
  }
  header .navbar ul li a {
    display: block;
    padding: 1rem;
    text-align: left;
    color: #fff;
    font-size: 2rem;
  }
  header .navbar ul li a.active,
  header .navbar ul li a:hover {
    padding: 1rem;
    color: #fff;
    border-radius: 0.5rem;
    border-bottom: 0.5rem solid #011aff;
  }
  .fa-times {
    transform: rotate(180deg);
  }
  header .navbar.nav-toggle {
    right: 0;
  }
}
/* hamburger icon ends */

/* hero section starts*/
.home {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  min-height: 100vh;
  align-items: center;
}
.home #particles-js {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}
.home::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}
.home .content {
  flex: 1 1 40rem;
  padding-top: 1rem;
  z-index: 1;
}
.home .image {
  flex: 1 1 40rem;
  z-index: 1;
}
.home .image img {
  width: 70%;
  margin-left: 6rem;
  border-radius: 50%;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
  cursor: pointer;
}
.home .image img:hover {
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
}
.home .content h2 {
  font-size: 5rem;
  font-weight: 800;
  color: #002057;
}
.home .content h2 span {
  font-size: 5rem;
  font-weight: 800;
  color: #ff7b00;
}
.home .content p {
  font-size: 2.5rem;
  color: #000;
  font-weight: 600;
  padding: 1rem 0;
}
.home .content p span {
  font-size: 2.5rem;
  color: rgb(148, 8, 8);
  font-weight: 600;
  padding: 1rem 0;
}
.home .btn {
  margin-top: 1rem;
  position: absolute;
  line-height: 0;
  padding: 1.6rem 3rem;
  border-radius: 4em;
  transition: 0.5s;
  color: #fff;
  background: #2506ad;
  box-shadow: 0px 5px 18px rgba(48, 68, 247, 0.6);
  font-family: "Nunito", sans-serif;
}
.home .btn span {
  font-weight: 700;
  font-size: 1.7rem;
  letter-spacing: 0.1rem;
}
.home .btn i {
  margin-left: 0.3rem;
  font-size: 1.5rem;
  transition: 0.3s;
}
.home .btn:hover {
  background: #1a047e;
}
.home .btn:hover i {
  transform: translateX(5px);
}
/* social icons start */
.socials {
  position: relative;
  margin-top: 9rem;
}
.socials .social-icons {
  padding-left: 0;
  margin-bottom: 0;
  list-style: none;
}
.socials .social-icons li {
  display: inline-block;
  margin-bottom: 14px;
}
.social-icons a {
  font-size: 2rem;
  display: inline-block;
  line-height: 44px;
  color: #00d9ff;
  background-color: #09011b;
  width: 44px;
  height: 44px;
  text-align: center;
  margin-right: 8px;
  border-radius: 100%;
  -webkit-transition: all 0.2s linear;
  -o-transition: all 0.2s linear;
  transition: all 0.2s linear;
}
.social-icons a:active,
.social-icons a:focus,
.social-icons a:hover {
  color: #fff;
  background-color: #0685da;
}
.social-icons a.github:hover {
  background-color: #0e0e0e;
}
.social-icons a.twitter:hover {
  background-color: #00aced;
}
.social-icons a.linkedin:hover {
  background-color: #007bb6;
}
.social-icons a.dev:hover {
  background-color: #070707;
}
.social-icons a.instagram:hover {
  background-color: #ee00da;
}
/* social icons end */

/* hero media queries starts*/
@media (max-width: 450px) {
  .home .btn {
    margin: 4rem 0;
  }
  .socials {
    margin-top: 12rem;
  }
  .home .image img {
    margin-top: -12rem;
  }
  .home .content p {
    font-size: 2.2rem;
  }
  .home .content p span {
    font-size: 2.2rem;
  }
}
/* hero media queries ends*/
/* hero section end */

/* about section starts */
.about {
  background: rgb(255, 255, 255);
}
.about .row {
  display: flex;
  flex-direction: row;
  gap: 2rem;
  flex-wrap: wrap;
  padding: 4rem;
}
.about .row .image {
  text-align: center;
  flex: 1 1 35rem;
}
.about .row .image img {
  margin: 4rem;
  width: 30rem;
  height: auto;
  border-radius: 5%;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.6);
  mix-blend-mode: luminosity;
  transition: 0.3s;
  cursor: pointer;
}
.about .row .image img:hover {
  mix-blend-mode: normal;
}
.about .row .content {
  flex: 1 1 45rem;
  padding: 3rem;
}
.about .row .content h3 {
  color: rgb(27, 27, 27);
  font-size: 2.5rem;
}
.about .row .content .tag {
  font-size: 1.4rem;
  color: #020133;
  font-weight: 600;
  margin-top: 1rem;
}
.about .row .content p {
  font-size: 1.5rem;
  margin-top: 1.5rem;
  font-family: "Nunito";
  font-weight: 600;
  text-transform: none;
}
.about .row .content .box-container {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  font-family: "Nunito";
  font-weight: 600;
}
.about .row .content .box-container .box p {
  text-transform: none;
}
.about .row .content .box-container .box p span {
  color: #011aff;
}
.resumebtn {
  margin-top: 6rem;
}
.resumebtn .btn {
  padding: 1.7rem 3rem;
  border-radius: 0.5em;
  transition: 0.3s;
  color: #fff;
  background: #2506ad;
  box-shadow: 0px 5px 10px rgba(48, 68, 247, 0.6);
  font-family: "Nunito", sans-serif;
}
.resumebtn .btn span {
  font-weight: 600;
  font-size: 1.8rem;
  letter-spacing: 0.1rem;
}
.resumebtn .btn i {
  margin-left: 0.3rem;
  font-size: 1.2rem;
  transition: 0.3s;
}
.resumebtn .btn:hover {
  background: #1a047e;
}
.resumebtn .btn:hover i {
  transform: translateX(5px);
}
/* about media queries starts*/
@media screen and (max-width: 600px) {
  .about .row .image {
    margin-top: 2rem;
  }
  .about .row .image img {
    margin: 0 auto;
    width: 80%;
    mix-blend-mode: normal;
  }
  .about .row {
    padding: 0.5rem;
    margin-bottom: 7rem;
  }
  .about .row .content {
    padding: 1rem;
  }
  .about .row .content .box-container {
    gap: 0;
  }
}
/* about media queries ends*/
/* about section ends */

/* skills section starts */
.skills {
  min-height: 90vh;
  background: linear-gradient(to bottom, #57059e, #4a00e0);
}
.skills h2 {
  color: #fff;
}
.skills .heading span {
  color: rgb(255, 230, 0);
}
.skills .container {
  background: rgba(0, 0, 22, 0.4);
  color: #fff;
  border-radius: 1rem;
  padding: 2rem;
  width: 90%;
  margin: auto;
  margin-top: 2rem;
}
.skills .container .row {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  flex-wrap: wrap;
  gap: 1.8rem;
}
.skills .container .bar {
  margin-bottom: 15px;
  padding: 10px;
  border-radius: 1rem;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  background: rgba(0, 0, 22, 0.9);
  transition: 0.2s;
}
.skills .container .bar:hover {
  box-shadow: 0 8px 10px rgba(0, 2, 68, 0.8) !important;
  background-color: rgba(0, 0, 0, 0.9) !important;
}
.skills .container .bar .info {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  margin-top: 1rem;
}
.skills .container .bar .info i {
  font-size: 4rem;
}
.skills .container .bar .info span {
  font-size: 2rem;
  font-weight: 500;
  font-family: "Poppins";
  margin-left: 0.5rem;
}
/* skills media queries starts*/
@media screen and (max-width: 600px) {
  .skills .container {
    padding: 0;
    margin: 0;
  }
  .skills .container .row {
    grid-template-columns: repeat(2, 1fr);
    margin: 1rem;
    padding: 2rem 0.2rem 2rem 0.2rem;
    gap: 1rem;
  }
  .skills .container {
    margin-top: 5px;
    width: 100%;
  }
}
/* skills media queries ends*/
/* skills section ends */

/* education section starts */
.education {
  background: #e5ecfb;
  min-height: 80vh;
}
.education .qoute {
  font-size: 1.5rem;
  text-align: center;
  font-family: "Nunito", sans-serif;
  font-weight: 600;
  margin-top: 0.5rem;
}
.education .box-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.education .box-container .box {
  display: flex;
  flex-direction: row;
  width: 80%;
  border-radius: 0.5rem;
  box-shadow: 0.2rem 0.5rem 1rem rgba(0, 0, 0, 0.2);
  text-align: center;
  position: relative;
  margin-top: 2rem;
  overflow: hidden;
  transition: 0.3s;
  background: rgb(252, 252, 252);
}
.education .box-container .box:hover {
  transform: scale(1.03);
  box-shadow: 1rem 0.5rem 1.2rem rgba(0, 0, 0, 0.3);
}
.education .box-container .box .image {
  flex: 1 1 20rem;
  width: 100%;
}
.education .box-container .box img {
  object-fit: cover;
  position: relative;
  width: 100%;
  height: 100%;
}
.education .box-container .box .content {
  position: relative;
  display: flex;
  flex-direction: column;
  padding: 1rem;
  flex-wrap: wrap;
  flex: 1 1 70rem;
}
.education .box-container .box .content h3 {
  font-size: 2.5rem;
  color: #012970;
  padding: 0.5rem 0;
  font-weight: 600;
  text-align: left;
  margin-left: 1rem;
}
.education .box-container .box .content p {
  font-size: 1.5rem;
  margin-left: 1rem;
  text-align: left;
}
.education h4 {
  font-size: 2rem;
  color: rgb(34, 109, 0);
  text-align: left;
  margin: 1rem;
  font-family: "Nunito", sans-serif;
  font-weight: 700;
}

/* education media queries starts*/
@media screen and (max-width: 600px) {
  .education .box-container .box {
    flex-direction: column;
    width: 100%;
  }
  .education .box-container .box .image {
    width: 100%;
    height: 25rem;
  }
  .education .box-container .box img {
    width: 100%;
  }
  .education .box-container .box .content {
    position: relative;
    display: flex;
    flex-direction: column;
    padding: 1rem;
    flex-wrap: wrap;
    flex: 0;
  }
  .education .btns {
    margin-top: 2rem;
    margin-left: 1rem;
    margin-right: 1rem;
    flex-wrap: wrap;
  }
}
/* education media queries ends*/
/* education section ends */

/* work section starts */
.work {
  /* background: #010124; */
  background: linear-gradient(to bottom, #000031, #00002c);
}
.work h2 {
  color: #fff;
  padding: 1rem;
}
.work .heading span {
  color: rgb(255, 230, 0);
}
.work .box-container {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  margin: 2rem;
}
.work .box-container .box {
  flex: 1 1 30rem;
  border-radius: 0.5rem;
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1);
  position: relative;
  overflow: hidden;
  height: 30rem;
}
.work .box-container .box img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
.work .box-container .box .content {
  height: 100%;
  width: 100%;
  position: absolute;
  top: 85%;
  left: 0;
  background: rgba(255, 255, 255, 0.9);
  display: flex;
  flex-direction: column;
}
.work .box-container .box .content .tag {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  height: 4.5rem;
  width: 100%;
  padding-left: 1rem;
  background: #ffd900;
}
.work .box-container .box .content .tag h3 {
  font-size: 2rem;
}
.work .box-container .box:hover .content {
  top: 25%;
}
.work .desc {
  margin: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.work .desc p {
  font-size: 1.5rem;
}
.work .desc .btns {
  display: flex;
  justify-content: space-between;
  width: 100%;
  margin-top: 2rem;
}
.work .desc .btns .btn {
  line-height: 0;
  display: inline;
  padding: 1.5rem 2.5rem;
  border-radius: 0.5rem;
  font-size: 1.5rem;
  color: #fff;
  background: rgb(12, 12, 12);
  margin-right: 2rem;
}
.work .desc .btns .btn:hover {
  background: #310ae0f5;
}
.work .viewall {
  display: flex;
  justify-content: center;
}
.work .viewall .btn {
  position: relative;
  line-height: 0;
  padding: 1.6rem 3rem;
  border-radius: 0.5em;
  transition: 0.5s;
  color: rgb(255, 255, 255);
  font-weight: 700;
  border: 2px solid #fff;
  box-shadow: 0px 5px 10px rgba(65, 84, 241, 0.4);
  text-align: center;
}
.work .viewall .btn span {
  font-weight: 600;
  font-size: 1.7rem;
  font-family: "Nunito", sans-serif;
}
.work .viewall .btn i {
  margin-left: 0.3rem;
  font-size: 1.5rem;
  transition: 0.3s;
}
.work .viewall .btn:hover {
  background: #fff;
  color: #000;
}
.work .viewall .btn:hover i {
  transform: translateX(5px);
}
/* work section ends */

/* experience section starts */
.experience .timeline {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}
.experience .timeline::after {
  content: "";
  position: absolute;
  width: 6px;
  background: #020133;
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -3px;
  z-index: -2;
}
.experience .container {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
}
/*circles on timeline*/
.experience .container::after {
  content: "\f0b1";
  position: absolute;
  width: 25px;
  height: 25px;
  right: -17px;
  background-color: rgb(255, 255, 255);
  border: 4px solid #ff9f55;
  top: 15px;
  border-radius: 50%;
  z-index: 100;
  font-size: 1.89rem;
  text-align: center;
  font-weight: 600;
  color: #02094b;
  font-family: "Font Awesome\ 5 Free";
}
.experience .left {
  left: 0;
}
.experience .right {
  left: 50%;
}
/* arrows pointing right */
.experience .left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid #f68c09;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent #f68c09;
}
/* arrows pointing left  */
.experience .right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid #f68c09;
  border-width: 10px 10px 10px 0;
  border-color: transparent #f68c09 transparent transparent;
}
.experience .right::after {
  left: -16px;
}
.experience .content {
  background-color: #f68c09;
  position: relative;
  border-radius: 6px;
}
.experience .content .tag {
  font-size: 1.3rem;
  padding-top: 1.5rem;
  padding-left: 1.5rem;
}
.experience .content .desc {
  margin-left: 1.5rem;
  padding-bottom: 1rem;
}
.experience .content .desc h3 {
  font-size: 1.5rem;
  font-weight: 600;
}
.experience .content .desc p {
  font-size: 1.2rem;
}
/* view all button */
.morebtn {
  display: flex;
  justify-content: center;
}
.morebtn .btn {
  position: relative;
  line-height: 0;
  padding: 1.6rem 3rem;
  border-radius: 0.5em;
  transition: 0.5s;
  color: #fff;
  background: #2506ad;
  box-shadow: 0px 5px 10px rgba(48, 68, 247, 0.6);
  text-align: center;
}
.morebtn .btn span {
  font-weight: 600;
  font-size: 1.7rem;
  font-family: "Nunito", sans-serif;
}
.morebtn .btn i {
  margin-left: 0.3rem;
  font-size: 1.5rem;
  transition: 0.3s;
}
.morebtn .btn:hover {
  background: #1a047e;
}
.morebtn .btn:hover i {
  transform: translateX(5px);
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
  .experience {
    min-height: 80vh;
  }
  .experience .timeline {
    margin-top: 2rem;
  }
  .experience .timeline::after {
    left: 31px;
  }
  .experience .container {
    width: 100%;
    padding-left: 8rem;
    padding-right: 2rem;
  }
  .experience .container::after {
    font-size: 2.2rem;
  }
  .experience .container::before {
    left: 61px;
    border: medium solid #f68c09;
    border-width: 10px 10px 10px 0;
    border-color: transparent #f68c09 transparent transparent;
  }
  .experience .left::after {
    left: 15px;
  }
  .experience .right::after {
    left: 15px;
  }
  .experience .right {
    left: 0%;
  }
  .morebtn {
    margin-top: 3rem;
  }
}
/* experience media queries ends */
/* experience section ends */

/* contact section starts */
.contact {
  background: #e5ecfb;
  min-height: 60vh;
}
.contact .container {
  max-width: 1050px;
  width: 100%;
  background: #fff;
  border-radius: 1.5rem;
  margin: 2rem 5rem;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.15);
}
.contact .container .content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 2.5rem 2rem;
}
.contact .content .image-box {
  max-width: 60%;
  margin-left: 4rem;
}
.contact .content .image-box img {
  width: 100%;
  height: 40rem;
  position: relative;
}
.contact .content form {
  width: 45%;
  margin-right: 3.5rem;
}
form .form-group {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.form-group .field {
  height: 50px;
  display: flex;
  position: relative;
  margin: 1rem;
  width: 100%;
}
form i {
  position: absolute;
  top: 50%;
  left: 18px;
  color: rgb(51, 51, 51);
  font-size: 17px;
  pointer-events: none;
  transform: translateY(-50%);
}
form .field input,
form .message textarea {
  width: 100%;
  height: 100%;
  outline: none;
  padding: 0 16px 0 48px;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
  border-radius: 5px;
  border: 1px solid rgb(51, 51, 51);
  background: #e5ecfb;
}
.field input::placeholder,
.message textarea::placeholder {
  color: rgb(51, 51, 51);
}
.field input:focus,
.message textarea:focus {
  padding-left: 47px;
  border: 2px solid rgb(115, 3, 167);
}
.field input:focus ~ i,
.message textarea:focus ~ i {
  color: rgb(115, 3, 167);
}
form .message {
  position: relative;
  margin: 1rem;
  width: 100%;
}
form .message i {
  top: 25px;
  font-size: 20px;
  left: 15px;
}
form .message textarea {
  min-height: 130px;
  max-height: 230px;
  max-width: 100%;
  min-width: 100%;
  padding: 12px 20px 0 48px;
}
form .message textarea::-webkit-scrollbar {
  width: 0px;
}
form .button-area {
  display: flex;
  float: right;
  flex-direction: row-reverse;
}
.button-area button {
  color: #fff;
  border: none;
  outline: none;
  font-size: 1.8rem;
  cursor: pointer;
  border-radius: 5px;
  padding: 13px 25px;
  background: #2506ad;
  box-shadow: 0px 5px 10px rgba(48, 68, 247, 0.6);
  transition: 0.3s ease;
  font-family: "Nunito", sans-serif;
}
.button-area button:hover {
  background: #421cecf5;
}
.button-area span {
  font-size: 17px;
  padding: 1rem;
  display: none;
}
.button-area button i {
  position: relative;
  top: 6px;
  left: 2px;
  font-size: 1.5rem;
  transition: 0.3s;
  color: #fff;
}
.button-area button:hover i {
  left: 8px;
}
/* contact section media queries starts */
@media (max-width: 900px) {
  .contact {
    min-height: 70vh;
  }
  .contact .container {
    margin: 3rem 0 2rem 0;
  }
  .contact .container .content {
    padding: 18px 12px;
  }
  .contact .content .image-box {
    display: none;
  }
  .contact .content form {
    width: 100%;
    margin-right: 2rem;
  }
}
/* contact section media queries ends */
/* contact section ends */

/* footer section starts */
.footer {
  min-height: auto;
  padding-top: 0;
  background: rgb(0, 1, 43);
}
.footer .box-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.footer .box-container .box {
  flex: 1 1 25rem;
  margin: 2.5rem;
}
.footer .box-container .box h3 {
  font-size: 2.5rem;
  color: #fff;
  padding-bottom: 1rem;
  font-weight: normal;
}
.footer .box-container .box p {
  font-size: 1.5rem;
  color: #ccc;
  padding: 0.7rem 0;
  text-transform: none;
}
.footer .box-container .box p i {
  padding-right: 1rem;
  color: #ffae00;
}
.footer .box-container .box a {
  font-size: 1.5rem;
  color: rgb(238, 238, 238);
  padding: 0.3rem 0;
  display: block;
}
.footer .box-container .box a:hover {
  color: #ffae00;
}
.footer .box-container .box .share {
  display: flex;
  flex-wrap: wrap;
  padding: 1rem 0;
}
.footer .box-container .box .share a {
  height: 4rem;
  width: 4rem;
  padding: 1rem;
  text-align: center;
  border-radius: 5rem;
  font-size: 1.7rem;
  margin-right: 1rem;
  transition: 0.2s;
  background: rgb(230, 230, 230);
  color: #02094b;
  border: none;
}
.footer .box-container .box .share a:hover {
  background: transparent;
  transform: scale(0.98);
  border: 0.1rem solid rgb(180, 178, 178);
  color: #ffae00;
}
.footer .credit {
  padding: 1rem 0 0 0;
  text-align: center;
  font-size: 1.5rem;
  font-family: "Nunito", sans-serif;
  font-weight: 600;
  color: #fff;
  border-top: 0.1rem solid #fff3;
}
.footer .credit a {
  color: #ffae00;
}
.footer .fa {
  color: #e90606;
  margin: 0 0.3rem;
  font-size: 1.5rem;
  animation: pound 0.35s infinite alternate;
}
@-webkit-keyframes pound {
  to {
    transform: scale(1.1);
  }
}
@keyframes pound {
  to {
    transform: scale(1.1);
  }
}
@media (max-width: 450px) {
  .footer .box-container .box {
    margin: 1.5rem;
  }
  .footer .box-container .box p {
    padding: 0.7rem;
  }
  .footer .box-container .box .share a {
    padding: 1.2rem;
  }
}
/* footer section ends */

/* common media queries starts*/
@media (max-width: 450px) {
  html {
    font-size: 55%;
  }
  body {
    padding-right: 0;
  }
  section {
    padding: 2rem;
  }
}
/* common media queries ends*/

/* scroll top starts */
#scroll-top {
  position: fixed;
  top: -140%;
  right: 2rem;
  padding: 1rem 1.5rem;
  font-size: 2rem;
  background: #ffae00;
  color: rgb(13, 0, 44);
  border-radius: 50%;
  transition: 1s linear;
  z-index: 1000;
}
#scroll-top.active {
  top: calc(100% - 12rem);
}
/* scroll top ends */
</style>

    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="keywords" content="Mohammed, portfolio, MOHAMMED, full stack dev, personal portfolio lifecodes, portfolio design, portfolio website, personal portfolio" />
    <meta name="description" content="Welcome to MOHAMMED's Portfolio. Full-Stack Web Developer and Android App Developer" />
    <!-- Custom CSS -->
    <link rel="stylesheet" href="./assets/css/style.css">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" integrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <!-- Favicon -->
    <link id='favicon' rel="shortcut icon" href="./assets/images/favicon.ico" type="image/x-png">
    <title>Portfolio | MOHAMMED OEDULLA</title>
    
    
    <!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-HTDER8P9VJ"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-HTDER8P9VJ');
</script>
    
    
</head>
<body oncontextmenu="return false">

<!-- pre loader -->
<!-- <div class="loader-container">
  <img draggable="false" src="./assets/images/preloader.gif" alt="">
</div> -->

<!-- navbar starts -->
<header>
        <a href="https://mohammedobedulla.github.io/web-portfolio/mohammedportfolio.html" class="logo"><i class="fab fa-node-js"></i> MOHAMMED</a>

        <div id="menu" class="fas fa-bars"></div>
        <nav class="navbar">
            <ul>
            <li><a class="active" href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#work">Work</a></li>
            <li><a href="#experience">Experience</a></li>
            </ul>
        </nav>
</header>
<!-- navbar ends -->


<!-- hero section starts -->
<section class="home" id="home">
    <div id="particles-js"></div>

    <div class="content">
    <h2>Hi There,<br/> I'm MOHAMMED <span>OBEDULLA</span></h2>
    <p>i am into <span class="typing-text"></span></p>
    <a href="#about" class="btn"><span>About Me</span>
      <i class="fas fa-arrow-circle-down"></i>
    </a>
    <div class="socials">
        <ul class="social-icons">
          <li><a class="linkedin" aria-label="LinkedIn" href="https://www.linkedin.com/in/mohammed-obedulla-905443178/" target="_blank"><i class="fab fa-linkedin"></i></a></li> 
          <li><a class="github" aria-label="GitHub" href="https://mohammedobedulla.github.io/web-portfolio/mohammedportfolio.html" target="_blank"><i class="fab fa-github"></i></a></li>
          <li><a class="twitter" aria-label="Twitter" href="https://twitter.com/MOHAMMEDOBEDUL4" target="_blank"><i class="fab fa-twitter"></i></a></li>
          <li><a class="telegram" aria-label="Telegram" href="https://t.me/MOHAMMEDOBEDULLA" target="_blank"><i class="fab fa-telegram-plane"></i></a></li>
          <li><a class="instagram" aria-label="Instagram" href="https://www.instagram.com/mohammedobedulla"><i class="fab fa-instagram" target="_blank"></i></a></li>
          </ul>
      </div>
    </div>
<div class="image">
    <img draggable="false" class="tilt" src="./assets/images/hero.png" alt="">
</div>
</section>
<!-- hero section ends -->


<!-- about section starts -->
<section class="about" id="about">
    <h2 class="heading"><i class="fas fa-user-alt"></i> About <span>Me</span></h2>
    
    <div class="row">

    <div class="image">
        <img draggable="false" class="tilt" src="./assets/images/profile2.jpg" alt="">
    </div>
    <div class="content">
        <h3>I'm MOHAMMED</h3>
        <span class="tag">Associate Software Engineer</span>
        
        <p>Am <b>Software Engineer</b> under professional at <b> Technology and Management.</b> 
          I am very passionate about improving my coding skills & developing native applications.
          I build Android Apps specially Native field.
          Working for myself to improve my skills.
          Love to build Full-Stack clones. </p>
        
        <div class="box-container">
            <div class="box">
              <p><span> age: </span> 24</p>
              <p><span> DOB: </span> 15-JULY-1997</p>
              <p><span> phone : </span> +91 9206971787</p>
            </div>
            <div class="box">
              <p><span> email : </span> moobjuly1997@gmail.com</p>
              <p><span> place : </span> Bangalore, India - 560049</p>
            </div>
        </div>
        
        <div class="resumebtn">
            <a href="https://www.linkedin.com/in/mohammed-obedulla-905443178" class="btn"><span>LinkedIn</span>
                <i class="fas fa-chevron-right"></i>
            </a>
        </div>

    </div>
    </div>
</section>
<!-- about section ends -->

<!-- skills section starts -->
<section class="skills" id="skills">

    <h2 class="heading"><i class="fas fa-laptop-code"></i> Skills & <span>Abilities</span></h2>

    <div class="container">
          <div class="row" id="skillsContainer">
            
            
            
            
            
            <!-- Start Skills Section -->

  <section id="skills" class="services">
    <div class="container">
      <div class="section-title">
        <h2>Skills</h2>
      </div>
      <div class="row">
        <div class="col-lg-12" data-aos="fade-up">
          <div class="col-md-12 mt-4 mt-md-0 icon-box" data-aos="fade-up" data-aos-delay="200" style="background:#fff">
            <h4 style="text-align:left;color:#09708a">Languages and Databases</h4>
                <p style="text-align:left;">
                  <img src="https://www.vectorlogo.zone/logos/python/python-horizontal.svg" alt="vectorlogo.zone" height="50" width="100">
                  <img src="https://www.vectorlogo.zone/logos/java/java-horizontal.svg" alt="vectorlogo.zone" height="50" width="150">
                  <img src="https://www.vectorlogo.zone/logos/w3_html5/w3_html5-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg" alt="upload.wikimedia.org" height="60" width="100">
                  <img src="https://www.vectorlogo.zone/logos/mysql/mysql-horizontal.svg" alt="vectorlogo.zone" height="70" width="130">
                  <img src="https://www.vectorlogo.zone/logos/postgresql/postgresql-horizontal.svg" alt="vectorlogo.zone" height="50" width="190">

                </p>
            </div>
            <p><div class="col-md-12 mt-4 mt-md-0 icon-box" data-aos="lefade-up" data-aos-delay="100" style="background:#fff">
              <h4 style="text-align:left;color:#09708a">Frameworks</h4>
                <p style="text-align:left;">
                  <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/djangoproject/djangoproject-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/nodejs/nodejs-horizontal.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/getbootstrap/getbootstrap-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/opencv/opencv-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="upload.wikimedia.org" width="90" height="70">
              </p>
          </div></p>
          <div class="col-md-12 mt-4 mt-md-0 icon-box" data-aos="lefade-up" data-aos-delay="100" style="background:#fff">
              <h4 style="text-align:left;color:#09708a">Tools</h4>
                <p style="text-align:left;">
                  <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/amazon_aws/amazon_aws-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/heroku/heroku-ar21.svg" alt="vectorlogo.zone">
                  <img src="https://www.vectorlogo.zone/logos/jupyter/jupyter-ar21.svg" alt="vectorlogo.zone">
              </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- End Skills Section -->
      </div>
</div>
</section>
<!-- skills section ends -->


<!-- my own notes section starts -->
<section class="skills" id="skills">

  <h2 class="heading"><i class="fas fa-book-open"></i> My Notes  <span>(Some imp Repo at GitHub)</span></h2>

  <div class="container">
        <div class="row" id="notesContainer">
          
          <h3><p><span><section id="skills" class="section scrollspy">
      <h2 class="page-title white-text teal">Skills</h2>
      <div class="container">
        
        <!-- Languages and Databases -->
        <div class="card">
          <div class="card-content">
            <h3 class="brown-text light">Languages and Databases</h3>
            <div class="row text-center">
              <div class="col s4 m2">
                <img alt="" src="/assets/img/python-logo-1-300x300.jpg" class="responsive-img" />Python
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/html5-300x300.jpg" class="responsive-img" />HTML5
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/css3-300x300.jpg" class="responsive-img" />CSS3
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/mysql-logo-1-300x300.jpg" class="responsive-img" />MySQL
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/postgresql-logo.png" class="responsive-img" />PostgreSQL
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/shell-logo-1-300x300.jpg" class="responsive-img" />Shell Scripting
              </div>
            </div>
          </div>
        </div>

        <div class="card">
          <div class="card-content">
            <h4 class="brown-text light">Libraries</h4>
            <div class="row text-center">
              <div class="col s4 m2">
                <img alt="" src="/assets/img/numpy-logo-1-500x500.jpg" class="responsive-img" />NumPy
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/pandas-logo-2-500x500.jpg" class="responsive-img" />Pandas
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/opencv-logo-1-500x500.jpg" class="responsive-img" />OpenCV
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/sk-learn-logo-1-500x500.jpg" class="responsive-img" />scikit-learn
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/matplotlib-logo-1-500x500.jpg" class="responsive-img" />matplotlib
              </div>
            </div>
          </div>
        </div>

        <!-- Frameworks -->
        <div class="card">
          <div class="card-content">
            <h4 class="brown-text light">Frameworks</h4>
            <div class="row text-center">
              <div class="col s4 m2">
                <img alt="" src="/assets/img/django-logo.webp" class="responsive-img" />Django
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/flask-logo.png" class="responsive-img" />Flask
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/bootstrap.png" class="responsive-img" />Bootstrap
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/keras-logo.png" class="responsive-img" />Keras
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/tensorflow-logo-1.png" class="responsive-img" />TensorFlow
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/pytorch-logo.png" class="responsive-img" />PyTorch
              </div>
            </div>
          </div>
        </div>

        <!-- Other -->
        <div class="card">
          <div class="card-content">
            <h4 class="brown-text light">Other</h4>
            <div class="row text-center">


              <div class="col s4 m2">
                <img alt="" src="/assets/img/git.png" class="responsive-img" />Git
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/aws.png" class="responsive-img" />AWS
              </div>
              <div class="col s4 m2">
                <img alt="" src="/assets/img/heroku.png" class="responsive-img" />Heroku
              </div>
            </div>
          </div>
        </div>
 </section>
       
         <!-- certifications -->
         <div class="card">
          <div class="card-content">
            <h4 class="brown-text light">Certificates</h4>
            <div class="row text-left">
              <div class="container">
                <div class="row">
                  <div class="col s12 m6 l6">
                    <div class="card">
                      <div class="card-image">
                        <img src="/assets/img/mooc-machine-learning-coursera-800x500.jpg">
                      </div>
                      <div class="card-content">
                        <span class="card-title teal-text">Machine Learning (Stanford)</span>
                      </div>
                    </div>
                  </div>
                  <div class="col s12 m6 l6">
                    <div class="card">
                      <div class="card-image">
                        <img src="/assets/img/mooc-algorithms-stanford-2-800x500.jpg">
                      </div>
                      <div class="card-content">
                        <span class="card-title teal-text">Algorithms (Stanford)</span>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div> -->

      </div>
            </section></h2>
       

    </div>
</div>
</section>
<!-- my own notes section ends -->



<!-- work project section starts -->
<section class="work" id="work">

  <h2 class="heading"><i class="fas fa-laptop-code"></i> Projects <span>Made</span></h2>

  <div class="box-container" id="projectsContainer">
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    


</div>

<div class="viewall">
  <a href="https://mohammedobedulla.github.io/web-portfolio/mohammedportfolio.html" class="btn"><span>View All</span>
    <i class="fas fa-arrow-right"></i>
</a>
</div>

</section>
<!-- work project section ends -->

<!-- experience section starts -->
<section class="experience" id="experience">

  <h2 class="heading"><i class="fas fa-briefcase"></i> Experience </h2>

  <div class="timeline">

    <div class="container right">
      <div class="content">
        <div class="tag">
          <h2>HackClub RAIT</h2>
        </div>
        <div class="desc">
            <h3>Project Mentor | Open Source</h3>
            <p>Jul 2022 - present</p>
        </div>
      </div>
    </div>

    <div class="container left">
      <div class="content">
        <div class="tag">
          <h2>GirsScript Summer of Code</h2>
        </div>
        <div class="desc">
            <h3>Contributor | Open Source</h3>
            <p>Mar 2022 - May 2022</p>
        </div>
      </div>
    </div>

    <div class="container right">
      <div class="content">
        <div class="tag">
          <h2>JGEC Winter of Code</h2>
        </div>
        <div class="desc">
            <h3>Project Mentor | Open Source</h3>
            <p>Feb 2022 - Mar 2022</p>
        </div>
      </div>
    </div>

    <div class="container left">
      <div class="content">
        <div class="tag">
          <h2>Rubberfy</h2>
        </div>
        <div class="desc">
            <h3>Mobile Application Developer | Internship</h3>
            <p>Nov 2021 - Dec 2021</p>
        </div>
      </div>
    </div>

  <div class="morebtn">
    <a href="experience/https://mohammedobedulla.github.io/web-portfolio/mohammedportfolio.html" class="btn"><span>View All</span>
      <i class="fas fa-arrow-right"></i>
  </a>
  </div>

</div>

</section>
<!-- experience section ends -->


<!-- education section starts -->
<section class="education" id="education">

  <h1 class="heading"><i class="fas fa-graduation-cap"></i> My <span>Education</span></h1>

    <p class="qoute">Education is not the learning of facts, but the training of the mind to think.</p>

    <div class="box-container">

    <div class="box">
        <div class="image">
        <img draggable="false" src="" alt="">
        </div>
        <div class="content">
        <h3>MCA</h3>
        <p>CMR Institite of technology</p>
        <p>8.75 CGPA till 6th Sem</p>
        <h4>2018-2020 | Completed</h4>
        </div>
    </div>

    <div class="box">
      <div class="image">
      <img src="\Users\moham\Downloads\CMRIT-NEW-LOGO-03-220x150-1.jpg" alt="">
      </div>
      <div class="content">
      <h3>BCA | COMPUTER APPLICATIONS </h3>
      <p>SDC COLLEGE KOLAR | FULL TIME</p>
      <p>85% |First class Disticntion</p>
      <h4>2015-2018 | Completed</h4>
      </div>
    </div>

    <div class="box">
      <div class="image">
      <img draggable="false" src="./assets/images/educat/bhimeswari.jpg" alt="">
      </div>
      <div class="content">
      <h3>12th | PCMB</h3>
      <p>Sri Venu Composite Pu College | PCMB</p>
      <p>57.4% in PCMB</p>
      <h4>2013-2015 | Completed</h4>
      </div>
    </div>

      
      <div class="box">
      <div class="image">
      <img src="C:\Users\moham\Downloads\CMRIT-NEW-LOGO-03-220x150-1.jpg" alt="">
      </div>
      <div class="content">
      <h3>SSCL | EDUCATOIN</h3>
      <p>Al Ameen high School |</p>
      <p>74.4% PCMB</p>
      <h4>2013 | Completed</h4>
      </div>
    </div>
      
</div>
</section>
<!-- education section ends -->


<!-- footer section starts -->
<section class="footer">

  <div class="box-container">

      <div class="box">
          <h3>MOHAMMED's Portfolio</h3>
          <p>Thank you for visiting my personal portfolio website. Connect with me over socials. <br/> <br/> Keep Rising 🚀. Connect with me over live chat!</p>
      </div>

      <div class="box">
          <h3>quick links</h3>
          <a href="#home"><i class="fas fa-chevron-circle-right"></i> home</a>
          <a href="#about"><i class="fas fa-chevron-circle-right"></i> about</a>
          <a href="#skills"><i class="fas fa-chevron-circle-right"></i> skills</a>
          <a href="#education"><i class="fas fa-chevron-circle-right"></i> education</a>
          <a href="#work"><i class="fas fa-chevron-circle-right"></i> work</a>
          <a href="#experience"><i class="fas fa-chevron-circle-right"></i> experience</a>
      </div>

      <div class="box">
          <h3>contact info</h3>
          <p> <i class="fas fa-phone"></i>+91 9206971787</p>
          <p> <i class="fas fa-envelope"></i>moobjuly1997@gmail.com</p>
          <p> <i class="fas fa-map-marked-alt"></i>Bangalore ,india 560049</p>
          <div class="share">

              <a href="https://www.linkedin.com/in/mohammed-obedulla-905443178" class="fab fa-linkedin" aria-label="LinkedIn" target="_blank"></a>
              <a href="https://mohammedobedulla.github.io/web-portfolio/mohammedportfolio.html/" class="fab fa-github" aria-label="GitHub" target="_blank"></a>
              <a href="mailto:moobjuly1997@gmail.com" class="fas fa-envelope" aria-label="Mail" target="_blank"></a>
              <a href="https://twitter.com/MOHAMMEDOBEDUL4" class="fab fa-twitter" aria-label="Twitter" target="_blank"></a>
          </div>
      </div>
  </div>
  
  
  
  
  <div class="col-xs-12 col-sm-8">
                                    <div id="map" class="map">
                                        <div class="lmpixels-map">
 <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d62199.59764448563!2d77.69046277370886!3d13.005404884290277!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bae11abc8ffe3e7%3A0xd8368746c98e53bf!2sKrishnarajapura%2C%20Bengaluru%2C%20Karnataka%2C%20India!5e0!3m2!1sen!2sus!4v1665554104667!5m2!1sen!2sus" width="600" height="300" style="border:50;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>">
                                        </div>
                                    </div>
  
  
  
  
  
  
  
  

  <h1 class="credit">Designed with <i class="fa fa-heart pulse"></i> by <a href="https://www.linkedin.com/in/www.linkedin.com/in/mohammed-obedulla-905443178"> MOHAMMED OBEDULLA</a></h1>

</style>



</section>
<!-- footer section ends -->


<!-- scroll top btn -->
<a href="#home" aria-label="ScrollTop" class="fas fa-angle-up" id="scroll-top"></a>
<!-- scroll back to top -->

<script>
$(document).ready(function () {

    $('#menu').click(function () {
        $(this).toggleClass('fa-times');
        $('.navbar').toggleClass('nav-toggle');
    });

    $(window).on('scroll load', function () {
        $('#menu').removeClass('fa-times');
        $('.navbar').removeClass('nav-toggle');

        if (window.scrollY > 60) {
            document.querySelector('#scroll-top').classList.add('active');
        } else {
            document.querySelector('#scroll-top').classList.remove('active');
        }

        // scroll spy
        $('section').each(function () {
            let height = $(this).height();
            let offset = $(this).offset().top - 200;
            let top = $(window).scrollTop();
            let id = $(this).attr('id');

            if (top > offset && top < offset + height) {
                $('.navbar ul li a').removeClass('active');
                $('.navbar').find(`[href="#${id}"]`).addClass('active');
            }
        });
    });

    // smooth scrolling
    $('a[href*="#"]').on('click', function (e) {
        e.preventDefault();
        $('html, body').animate({
            scrollTop: $($(this).attr('href')).offset().top,
        }, 500, 'linear')
    });

    // <!-- emailjs to mail contact form data -->
    $("#contact-form").submit(function (event) {
        emailjs.init("user_TTDmetQLYgWCLzHTDgqxm");

        emailjs.sendForm('contact_service', 'template_contact', '#contact-form')
            .then(function (response) {
                console.log('SUCCESS!', response.status, response.text);
                document.getElementById("contact-form").reset();
                alert("Form Submitted Successfully");
            }, function (error) {
                console.log('FAILED...', error);
                alert("Form Submission Failed! Try Again");
            });
        event.preventDefault();
    });
    // <!-- emailjs to mail contact form data -->

});

document.addEventListener('visibilitychange',
    function () {
        if (document.visibilityState === "visible") {
            document.title = "Portfolio | MOHAMMED OBEDULLA";
            $("#favicon").attr("href", "assets/images/favicon.ico");
        }
        else {
            document.title = "Portfolio |MOHAMMED OBEDULLA";
            $("#favicon").attr("href", "assets/images/favicon.ico");
        }
    });


// <!-- typed js effect starts -->
var typed = new Typed(".typing-text", {
    strings: ["android development", "web development" , "backend development"],
    loop: true,
    typeSpeed: 50,
    backSpeed: 25,
    backDelay: 500,
});
// <!-- typed js effect ends -->

async function fetchData(type = "skills") {
    let response
    if(type==="skills"){
        response = await fetch("skills.json")
    }else if(type === "projects"){
        response = await fetch("./projects/projects.json")
    }else if(type==="notes"){
        response = await fetch("dsa.json")
    }
    const data = await response.json();
    return data;
}

function showSkills(skills) {
    let skillsContainer = document.getElementById("skillsContainer");
    let skillHTML = "";
    skills.forEach(skill => {
        skillHTML += `
        <div class="bar">
              <div class="info">
                <img src=${skill.icon} alt="skill" />
                <span>${skill.name}</span>
              </div>
            </div>`
    });
    skillsContainer.innerHTML = skillHTML;
}

function showNotes(notes) {
    let skillsContainer = document.getElementById("notesContainer");
    let skillHTML = "";
    notes.forEach(skill => {
        skillHTML += `
        <div class="bar">
              <div class="info">
                <a target="_blank" href=${skill.link}>
                <img src=${skill.icon} alt="skill"/></a>
                <span>${skill.name}</span>
              </div>
            </div>`
    });
    skillsContainer.innerHTML = skillHTML;
}

function showProjects(projects) {
    let projectsContainer = document.querySelector("#work .box-container");
    let projectHTML = "";
    projects.slice(0, 10).filter(project => project.category != "android").forEach(project => {
        projectHTML += `
        <div class="box tilt">
      <img draggable="false" src="assets/images/projects/${project.image}.png" alt="project" />
      <div class="content">
        <div class="tag">
        <h3>${project.name}</h3>
        </div>
        <div class="desc">
          <p>${project.desc}</p>
          <div class="btns">
            <a href="${project.links.view}" class="btn" target="_blank"><i class="fas fa-eye"></i> View</a>
            <a href="${project.links.code}" class="btn" target="_blank">Code <i class="fas fa-code"></i></a>
          </div>
        </div>
      </div>
    </div>`
    });
    projectsContainer.innerHTML = projectHTML;

    // <!-- tilt js effect starts -->
    VanillaTilt.init(document.querySelectorAll(".tilt"), {
        max: 15,
    });
    // <!-- tilt js effect ends -->

    /* ===== SCROLL REVEAL ANIMATION ===== */
    const srtop = ScrollReveal({
        origin: 'top',
        distance: '80px',
        duration: 1000,
        reset: true
    });

    /* SCROLL PROJECTS */
    srtop.reveal('.work .box', { interval: 200 });

}

fetchData().then(data => {
    showSkills(data);
});

fetchData("projects").then(data => {
    showProjects(data);
});

fetchData("notes").then(data => {
    showNotes(data);
});

// <!-- tilt js effect starts -->
VanillaTilt.init(document.querySelectorAll(".tilt"), {
    max: 15,
});
// <!-- tilt js effect ends -->



document.onkeydown = function (e) {
    if (e.keyCode == 123) {
        return false;
    }
    if (e.ctrlKey && e.shiftKey && e.keyCode == 'I'.charCodeAt(0)) {
        return false;
    }
    if (e.ctrlKey && e.shiftKey && e.keyCode == 'C'.charCodeAt(0)) {
        return false;
    }
    if (e.ctrlKey && e.shiftKey && e.keyCode == 'J'.charCodeAt(0)) {
        return false;
    }
    if (e.ctrlKey && e.keyCode == 'U'.charCodeAt(0)) {
        return false;
    }
}



/* ===== SCROLL REVEAL ANIMATION ===== */
const srtop = ScrollReveal({
    origin: 'top',
    distance: '80px',
    duration: 1000,
    reset: true
});

/* SCROLL HOME */
srtop.reveal('.home .content h3', { delay: 200 });
srtop.reveal('.home .content p', { delay: 200 });
srtop.reveal('.home .content .btn', { delay: 200 });

srtop.reveal('.home .image', { delay: 400 });
srtop.reveal('.home .linkedin', { interval: 600 });
srtop.reveal('.home .github', { interval: 800 });
srtop.reveal('.home .twitter', { interval: 1000 });
srtop.reveal('.home .telegram', { interval: 600 });
srtop.reveal('.home .instagram', { interval: 600 });
srtop.reveal('.home .dev', { interval: 600 });

/* SCROLL ABOUT */
srtop.reveal('.about .content h3', { delay: 200 });
srtop.reveal('.about .content .tag', { delay: 200 });
srtop.reveal('.about .content p', { delay: 200 });
srtop.reveal('.about .content .box-container', { delay: 200 });
srtop.reveal('.about .content .resumebtn', { delay: 200 });


/* SCROLL SKILLS */
srtop.reveal('.skills .container', { interval: 200 });
srtop.reveal('.skills .container .bar', { delay: 400 });

/* SCROLL EDUCATION */
srtop.reveal('.education .box', { interval: 200 });

/* SCROLL PROJECTS */
srtop.reveal('.work .box', { interval: 200 });

/* SCROLL EXPERIENCE */
srtop.reveal('.experience .timeline', { delay: 400 });
srtop.reveal('.experience .timeline .container', { interval: 400 });

/* SCROLL CONTACT */
srtop.reveal('.contact .container', { delay: 400 });
srtop.reveal('.contact .container .form-group', { delay: 400 });
</script>


</body>
</html>
