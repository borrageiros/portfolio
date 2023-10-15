<script>
    import SkillMeter from '../../components/SkillMeter.svelte';
</script>
<div id="content">
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
                <pre>jul 2023 / NOW  -  Full Stack Developer on an internship with a scholarship at NetexLearning</pre>
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
                <h1>JS</h1><br>
                <svg>
                    <SkillMeter percentage={75} />
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



        <!-- CISCO COURSES -->
        <h1>Cisco Courses</h1>
        <hr><br><br>
        <div class="cisco-courses">
            <table>
                <tr>
                    <td>
                        <h3>Python Essentials 1</h3><br>
                        <img src="/cisco/python1.png" alt="Python Essentials 1">
                    </td>
                    <td>
                        <h3>Python Essentials 2</h3><br>
                        <img src="/cisco/python2.png" alt="Python Essentials 2">
                    </td>
                    <td>
                        <h3>Endpoint Security</h3><br>
                        <img src="/cisco/EndpointSecurity.png" alt="Endpoint Security">
                    </td>
                </tr>
                <tr>
                    <td>
                        <h3>Networking <br>basics</h3><br>
                        <img src="/cisco/NetworkingBasics.png" alt="Introducion to Networking">
                    </td>
                    <td>
                        <h3>Introduction <br>to Cybersecurity</h3><br>
                        <img src="/cisco/IntroductionSecurity.png" alt="Introduction to Cybersecurity">
                    </td>
                    <td>
                        <h3>Introducion <br>to Data Science</h3><br>
                        <img src="/cisco/IntroductionDataScience.png" alt="Introducion to Data Science">
                    </td>
                </tr>
                <tr>
                    <td>
                        <h3>Introduction <br>to Cisco Packet Tracer</h3><br>
                        <img src="/cisco/PacketTracer.png" alt="Introduction to Cisco Packet Tracer">
                    </td>
                    <td></td>
                    <td></td>
                </tr>
            </table>
        </div>



        <!-- COMPLEMENTARY -->
        <h1>Complementary</h1>
        <hr><br><br>
        <div class="about-me">
            <p>2017 - Car license</p>
            <p>Food handler</p>
            <p>Programing courses on Udemy</p>
            <p>Intermediate proficiency in image (Adobe Photoshop) or video edit</p>
        </div>
    </div>
</div>