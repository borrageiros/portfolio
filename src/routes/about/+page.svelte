<script>
    import SkillMeter from '../../components/SkillMeter.svelte';
</script>
<style>
    /* progress bar */
    svg {
        width: 114px;
        height: 114px;
        margin: 1em;
    }
    .skills{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        margin-bottom: 10vh;
    }
    .skill{
        text-align: center;
    }


    /* ABOUT ME */
    .about-me{
        margin-bottom: 10vh;
    }
    .about-me, hr{
        margin-bottom: 2vh;
    }
    .about-me h4, p:first-child{
        margin-top: 2vh;
    }
    pre {
        white-space: pre-wrap;
        word-wrap: break-word;
        margin-right: 20px;
    }



    /* LANGUAGES */
    .languages{
        width: 100%;
        text-align: center;
    }
    .languages .title{
        padding: 2vh;
    }

    /* CISCO COURSES */
    .certifications:first-child(table){
        margin-bottom: 10vh;
    }
    .certifications table{
        width: 100%;
        text-align: center;
    }
    .certifications td{
        padding-top: 3%;
    }
    .certifications img{
        width: 150px;
    }

    .languages, .certifications {
        overflow-x: auto;
        display: block;
    }
    .certifications img {
        width: 100%;
        max-width: 150px;
        height: auto;
    }
    .languages td, .certifications td {
        padding: 5px;
        margin: 0;
    }



    @media only screen and (max-width: 768px) {
        pre{
            margin-left: 4vh;
        }
        h1, h4{
            margin-left: 1vh;
        }
        .content{
            margin-top: 15vh;
        }
        .languages td, .certifications td {
            font-size: 0.8em;
        }
        .skills {
            flex-direction: column;
            align-items: center;
        }
        .skills svg {
            margin-bottom: 7vh;
        }
        .languages, .certifications table {
            width: 100%;
            overflow-x: auto;
        }
    }
</style>
<div class="content">
    <!-- ABOUT ME -->
    <div class="about-me">
        <h1>About me</h1>
        <hr>
        <pre>   I am a highly motivated individual with a strong passion for computer science. I have experience in various programming languages such as Python, JavaScript and PHP. I am eager to enter the workforce and put my knowledge to use in the field of programming.I am confident that my skills and determination will make me a valuable asset to any team.Currently, I am working as a full stack developer intern with a paid university scholarship at a company called NetexLearning.</pre>
        <h4>Education</h4>
        <hr>
        <div>
            <pre>sep 2021 / jun 2023  -  Desarrollo de Aplicaciones Web  -  Centro de Formación Profesional Afundación</pre>
            <pre>sep 2018 / jun 2020  -  Sistemas microinformáticos y redes  -  IES Fernando Wirtz Suarez</pre>
        </div>
        <h4>Works</h4>
        <hr>
        <div>
            <pre>march 2023 / NOW  -  Full Stack Developer on an internship with a scholarship at <a href="https://www.netexlearning.com/">NetexLearning</a></pre>
        </div>
    </div>



    <!-- LANGUAGES -->
    <h1>Languages</h1>
    <hr>
    <div class="skills">
        <table class="languages">

            <tr>
                <td></td>
                <td class="title"><h1>Oral <br> comprehension</h1></td>
                <td class="title"><h1>Speaking</h1></td>
                <td class="title"><h1>Reading <br> comprehension</h1></td>
                <td class="title"><h1>Writing</h1></td>
            </tr>
            
            <!-- SPANISH -->
            <tr>
                <td>Spanish</td>
                <!-- oral comprehension -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
                <!-- speaking -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
                <!-- reading comprehesion -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
                <!-- writing -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
            </tr>

            <!-- ENGLISH -->
            <tr>
                <td>English</td>
                <!-- oral comprehension -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={75} />
                        </svg>
                    </div>
                </td>
                <!-- speaking -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={35} />
                        </svg>
                    </div>
                </td>
                <!-- reading comprehesion -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={75} />
                        </svg>
                    </div>
                </td>
                <!-- writing -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={70} />
                        </svg>
                    </div>
                </td>
            </tr>

            <!-- GALICIAN -->
            <tr>
                <td>Galician</td>
                <!-- oral comprehension -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
                <!-- speaking -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={80} />
                        </svg>
                    </div>
                </td>
                <!-- reading comprehesion -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={100} />
                        </svg>
                    </div>
                </td>
                <!-- writing -->
                <td>
                    <div class="skill">
                        <svg>
                            <SkillMeter percentage={65} />
                        </svg>
                    </div>
                </td>
            </tr>
        </table>
    </div>



    <!-- SKILLS -->
    <h1>Skills</h1>
    <hr><br><br>
    <div class="skills">

        <div class="skill">
            <h1>Teamwork</h1><br>
            <svg>
                <SkillMeter percentage={65} />
            </svg>
        </div>

        <div class="skill">
            <h1>Problem Solving</h1><br>
            <svg>
                <SkillMeter percentage={90} />
            </svg>
        </div>

        <div class="skill">
            <h1>Adaptability</h1><br>
            <svg>
                <SkillMeter percentage={90} />
            </svg>
        </div>

        <div class="skill">
            <h1>Creativity</h1><br>
            <svg>
                <SkillMeter percentage={85} />
            </svg>
        </div>

        <div class="skill">
            <h1>Time Management</h1><br>
            <svg>
                <SkillMeter percentage={75} />
            </svg>
        </div>

    </div>



    <!-- LANGUAGES -->
    <h1>Informatic Languages</h1>
    <hr><br><br>
    <div class="skills">
        <div class="skill">
            <h1>Python</h1><br>
            <svg>
                <SkillMeter percentage={65} />
            </svg>
        </div>

        <div class="skill">
            <h1>HTML</h1><br>
            <svg>
                <SkillMeter percentage={90} />
            </svg>
        </div>

        <div class="skill">
            <h1>CSS</h1><br>
            <svg>
                <SkillMeter percentage={75} />
            </svg>
        </div>

        <div class="skill">
            <h1>JavaScript</h1><br>
            <svg>
                <SkillMeter percentage={75} />
            </svg>
        </div>

        <div class="skill">
            <h1>TypeScript</h1><br>
            <svg>
                <SkillMeter percentage={30} />
            </svg>
        </div>

        <div class="skill">
            <h1>PHP</h1><br>
            <svg>
                <SkillMeter percentage={30} />
            </svg>
        </div>

        <div class="skill">
            <h1>Java</h1><br>
            <svg>
                <SkillMeter percentage={30} />
            </svg>
        </div>

    </div>



    <!-- CERTIFICATIONS -->
    <h1>Certifications</h1>
    <hr><br/><br/><br/>

    <h3>Google</h3>
    <hr>
    <div class="certifications">
        <table>
            <tr>
                <td>
                    <h3>Analytics <br>Academy for Beginners</h3><br>
                    <img src="/certifications_icons/google/google_analytics_academy_beginners.jpg" alt="Analytics Academy for Beginners">               
                </td>
            </tr>
        </table>
    </div>

    <h3>MongoDB</h3>
    <hr>
    <div class="certifications">
        <table>
            <tr>
                <td>
                    <h3>MongoDB Node.js <br>Developer Path</h3><br>
                    <img src="/certifications_icons/mongodb/mongodb_nodejs_certification.jpg" alt="MongoDB Node.js Developer Path">               
                </td>
            </tr>
        </table>
    </div>

    <h3>Cisco</h3>
    <hr>
    <div class="certifications">
        <table>
            <tr>
                <td>
                    <h3>Python Essentials 1</h3><br>
                    <img src="/certifications_icons/cisco/python1.png" alt="Python Essentials 1">
                </td>
                <td>
                    <h3>Python Essentials 2</h3><br>
                    <img src="/certifications_icons/cisco/python2.png" alt="Python Essentials 2">
                </td>
                <td>
                    <h3>Endpoint Security</h3><br>
                    <img src="/certifications_icons/cisco/EndpointSecurity.png" alt="Endpoint Security">
                </td>
            </tr>
            <tr>
                <td>
                    <h3>Networking <br>basics</h3><br>
                    <img src="/certifications_icons/cisco/NetworkingBasics.png" alt="Introducion to Networking">
                </td>
                <td>
                    <h3>Introduction <br>to Cybersecurity</h3><br>
                    <img src="/certifications_icons/cisco/IntroductionSecurity.png" alt="Introduction to Cybersecurity">
                </td>
                <td>
                    <h3>Introducion <br>to Data Science</h3><br>
                    <img src="/certifications_icons/cisco/IntroductionDataScience.png" alt="Introducion to Data Science">
                </td>
            </tr>
            <tr>
                <td>
                    <h3>Introduction <br>to Cisco Packet Tracer</h3><br>
                    <img src="/certifications_icons/cisco/PacketTracer.png" alt="Introduction to Cisco Packet Tracer">
                </td>
                <td></td>
                <td></td>
            </tr>
        </table>
    </div>

    <h3>FreeCodeCamp</h3>
    <hr>
    <div class="certifications">
        <table>
            <tr>
                <td>
                    <h3>Responsive <br>Web Design</h3><br>
                    <svg aria-hidden="true" viewBox="0 0 640 512" xmlns="http://www.w3.org/2000/svg" class="map-icon">
                        <path d="M112 48h352v48h48V32a32.09 32.09 0 00-32-32H96a32.09 32.09 0 00-32 32v256H16a16 16 0 00-16 16v16a64.14 64.14 0 0063.91 64H352v-96H112zm492 80H420a36 36 0 00-36 36v312a36 36 0 0036 36h184a36 36 0 0036-36V164a36 36 0 00-36-36zm-12 336H432V176h160z"></path>
                    </svg>                        
                </td>
                <td>
                    <h3>JavaScript Algorithms <br>and <br>Data Structures</h3><br>
                    <svg aria-hidden="true" viewBox="0 0 448 512" xmlns="http://www.w3.org/2000/svg" class="map-icon">
                        <path d="M0 32v448h448V32H0zm243.8 349.4c0 43.6-25.6 63.5-62.9 63.5-33.7 0-53.2-17.4-63.2-38.5l34.3-20.7c6.6 11.7 12.6 21.6 27.1 21.6 13.8 0 22.6-5.4 22.6-26.5V237.7h42.1v143.7zm99.6 63.5c-39.1 0-64.4-18.6-76.7-43l34.3-19.8c9 14.7 20.8 25.6 41.5 25.6 17.4 0 28.6-8.7 28.6-20.8 0-14.4-11.4-19.5-30.7-28l-10.5-4.5c-30.4-12.9-50.5-29.2-50.5-63.5 0-31.6 24.1-55.6 61.6-55.6 26.8 0 46 9.3 59.8 33.7L368 290c-7.2-12.9-15-18-27.1-18-12.3 0-20.1 7.8-20.1 18 0 12.6 7.8 17.7 25.9 25.6l10.5 4.5c35.8 15.3 55.9 31 55.9 66.2 0 37.8-29.8 58.6-69.7 58.6z"></path>
                    </svg>                        
                </td>
                <td>
                    <h3>Front End <br>Development Libraries</h3><br>
                    <svg aria-hidden="true" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg" class="map-icon">
                        <path d="M418.2 177.2c-5.4-1.8-10.8-3.5-16.2-5.1.9-3.7 1.7-7.4 2.5-11.1 12.3-59.6 4.2-107.5-23.1-123.3-26.3-15.1-69.2.6-112.6 38.4-4.3 3.7-8.5 7.6-12.5 11.5-2.7-2.6-5.5-5.2-8.3-7.7-45.5-40.4-91.1-57.4-118.4-41.5-26.2 15.2-34 60.3-23 116.7 1.1 5.6 2.3 11.1 3.7 16.7-6.4 1.8-12.7 3.8-18.6 5.9C38.3 196.2 0 225.4 0 255.6c0 31.2 40.8 62.5 96.3 81.5 4.5 1.5 9 3 13.6 4.3-1.5 6-2.8 11.9-4 18-10.5 55.5-2.3 99.5 23.9 114.6 27 15.6 72.4-.4 116.6-39.1 3.5-3.1 7-6.3 10.5-9.7 4.4 4.3 9 8.4 13.6 12.4 42.8 36.8 85.1 51.7 111.2 36.6 27-15.6 35.8-62.9 24.4-120.5-.9-4.4-1.9-8.9-3-13.5 3.2-.9 6.3-1.9 9.4-2.9 57.7-19.1 99.5-50 99.5-81.7 0-30.3-39.4-59.7-93.8-78.4zM282.9 92.3c37.2-32.4 71.9-45.1 87.7-36 16.9 9.7 23.4 48.9 12.8 100.4-.7 3.4-1.4 6.7-2.3 10-22.2-5-44.7-8.6-67.3-10.6-13-18.6-27.2-36.4-42.6-53.1 3.9-3.7 7.7-7.2 11.7-10.7zM167.2 307.5c5.1 8.7 10.3 17.4 15.8 25.9-15.6-1.7-31.1-4.2-46.4-7.5 4.4-14.4 9.9-29.3 16.3-44.5 4.6 8.8 9.3 17.5 14.3 26.1zm-30.3-120.3c14.4-3.2 29.7-5.8 45.6-7.8-5.3 8.3-10.5 16.8-15.4 25.4-4.9 8.5-9.7 17.2-14.2 26-6.3-14.9-11.6-29.5-16-43.6zm27.4 68.9c6.6-13.8 13.8-27.3 21.4-40.6s15.8-26.2 24.4-38.9c15-1.1 30.3-1.7 45.9-1.7s31 .6 45.9 1.7c8.5 12.6 16.6 25.5 24.3 38.7s14.9 26.7 21.7 40.4c-6.7 13.8-13.9 27.4-21.6 40.8-7.6 13.3-15.7 26.2-24.2 39-14.9 1.1-30.4 1.6-46.1 1.6s-30.9-.5-45.6-1.4c-8.7-12.7-16.9-25.7-24.6-39s-14.8-26.8-21.5-40.6zm180.6 51.2c5.1-8.8 9.9-17.7 14.6-26.7 6.4 14.5 12 29.2 16.9 44.3-15.5 3.5-31.2 6.2-47 8 5.4-8.4 10.5-17 15.5-25.6zm14.4-76.5c-4.7-8.8-9.5-17.6-14.5-26.2-4.9-8.5-10-16.9-15.3-25.2 16.1 2 31.5 4.7 45.9 8-4.6 14.8-10 29.2-16.1 43.4zM256.2 118.3c10.5 11.4 20.4 23.4 29.6 35.8-19.8-.9-39.7-.9-59.5 0 9.8-12.9 19.9-24.9 29.9-35.8zM140.2 57c16.8-9.8 54.1 4.2 93.4 39 2.5 2.2 5 4.6 7.6 7-15.5 16.7-29.8 34.5-42.9 53.1-22.6 2-45 5.5-67.2 10.4-1.3-5.1-2.4-10.3-3.5-15.5-9.4-48.4-3.2-84.9 12.6-94zm-24.5 263.6c-4.2-1.2-8.3-2.5-12.4-3.9-21.3-6.7-45.5-17.3-63-31.2-10.1-7-16.9-17.8-18.8-29.9 0-18.3 31.6-41.7 77.2-57.6 5.7-2 11.5-3.8 17.3-5.5 6.8 21.7 15 43 24.5 63.6-9.6 20.9-17.9 42.5-24.8 64.5zm116.6 98c-16.5 15.1-35.6 27.1-56.4 35.3-11.1 5.3-23.9 5.8-35.3 1.3-15.9-9.2-22.5-44.5-13.5-92 1.1-5.6 2.3-11.2 3.7-16.7 22.4 4.8 45 8.1 67.9 9.8 13.2 18.7 27.7 36.6 43.2 53.4-3.2 3.1-6.4 6.1-9.6 8.9zm24.5-24.3c-10.2-11-20.4-23.2-30.3-36.3 9.6.4 19.5.6 29.5.6 10.3 0 20.4-.2 30.4-.7-9.2 12.7-19.1 24.8-29.6 36.4zm130.7 30c-.9 12.2-6.9 23.6-16.5 31.3-15.9 9.2-49.8-2.8-86.4-34.2-4.2-3.6-8.4-7.5-12.7-11.5 15.3-16.9 29.4-34.8 42.2-53.6 22.9-1.9 45.7-5.4 68.2-10.5 1 4.1 1.9 8.2 2.7 12.2 4.9 21.6 5.7 44.1 2.5 66.3zm18.2-107.5c-2.8.9-5.6 1.8-8.5 2.6-7-21.8-15.6-43.1-25.5-63.8 9.6-20.4 17.7-41.4 24.5-62.9 5.2 1.5 10.2 3.1 15 4.7 46.6 16 79.3 39.8 79.3 58 0 19.6-34.9 44.9-84.8 61.4zm-149.7-15c25.3 0 45.8-20.5 45.8-45.8s-20.5-45.8-45.8-45.8c-25.3 0-45.8 20.5-45.8 45.8s20.5 45.8 45.8 45.8z"></path>
                    </svg>                      
                </td>
            </tr>
            <tr>
                <td>
                    <h3>Data Visualization</h3><br>
                    <svg aria-hidden="true" viewBox="-10 -10 116 111" xmlns="http://www.w3.org/2000/svg" class="map-icon">
                        <path d="M0 0h7.75a45.5 45.5 0 110 91H0V71h7.75a25.5 25.5 0 100-51H0zm36.251 0h32a27.75 27.75 0 0121.331 45.5A27.75 27.75 0 0168.251 91h-32a53.69 53.69 0 0018.746-20H68.25a7.75 7.75 0 100-15.5H60.5a53.69 53.69 0 000-20h7.75a7.75 7.75 0 100-15.5H54.997A53.69 53.69 0 0036.251 0z"></path>
                    </svg>
                </td>
                <td>
                    <h3>Back End Development <br>and APIs</h3><br>
                    <svg aria-hidden="true" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg" class="map-icon">
                        <path d="M424 400c0 13.255-10.745 24-24 24s-24-10.745-24-24 10.745-24 24-24 24 10.745 24 24zm-88-24c-13.255 0-24 10.745-24 24s10.745 24 24 24 24-10.745 24-24-10.745-24-24-24zm64-144c-13.255 0-24 10.745-24 24s10.745 24 24 24 24-10.745 24-24-10.745-24-24-24zm-64 0c-13.255 0-24 10.745-24 24s10.745 24 24 24 24-10.745 24-24-10.745-24-24-24zm176-72a47.758 47.758 0 01-6.438 24A47.758 47.758 0 01512 208v96a47.758 47.758 0 01-6.438 24A47.758 47.758 0 01512 352v96c0 26.51-21.49 48-48 48H48c-26.51 0-48-21.49-48-48v-96a47.758 47.758 0 016.438-24A47.758 47.758 0 010 304v-96a47.758 47.758 0 016.438-24A47.758 47.758 0 010 160V64c0-26.51 21.49-48 48-48h416c26.51 0 48 21.49 48 48v96zm-464 0h416V64H48v96zm416 48H48v96h416v-96zm0 144H48v96h416v-96zm-64-216c13.255 0 24-10.745 24-24s-10.745-24-24-24-24 10.745-24 24 10.745 24 24 24zm-64 0c13.255 0 24-10.745 24-24s-10.745-24-24-24-24 10.745-24 24 10.745 24 24 24z"></path>
                    </svg>
                </td>
            </tr>
        </table>
    </div>

    <!-- COMPLEMENTARY -->
    <h1>Complementary</h1>
    <hr>
    <div>
        <p>2017 - Car license</p>
        <p>Food handler</p>
        <p>Programing courses on Udemy</p>
        <p>Intermediate proficiency in image (Adobe Photoshop) or video edit</p>
    </div>
</div>