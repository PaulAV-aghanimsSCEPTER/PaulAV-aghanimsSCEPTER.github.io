
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        :root {
            --primary: hsl(222.2 47.4% 11.2%);
            --primary-foreground: hsl(210 40% 98%);
            --background: hsl(0 0% 100%);
            --foreground: hsl(222.2 47.4% 11.2%);
            --muted: hsl(210 40% 96.1%);
            --muted-foreground: hsl(215.4 16.3% 46.9%);
            --accent: hsl(210 40% 96.1%);
            --accent-foreground: hsl(222.2 47.4% 11.2%);
        }

        @media (prefers-color-scheme: dark) {
            :root {
                --primary: hsl(210 40% 98%);
                --primary-foreground: hsl(222.2 47.4% 11.2%);
                --background: hsl(222.2 47.4% 11.2%);
                --foreground: hsl(210 40% 98%);
                --muted: hsl(217.2 32.6% 17.5%);
                --muted-foreground: hsl(215 20.2% 65.1%);
                --accent: hsl(217.2 32.6% 17.5%);
                --accent-foreground: hsl(210 40% 98%);
            }
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--background);
            color: var(--foreground);
            line-height: 1.5;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 64rem;
            margin: 0 auto;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 3rem;
        }

        h1 {
            font-size: 2.5rem;
            font-weight: 700;
        }

        .logo {
            width: 6rem;
            height: 6rem;
            object-fit: contain;
        }

        .section {
            background-color: var(--accent);
            border-radius: 0.5rem;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
        }

        h2 {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            text-align: center;
            color: var(--primary);
        }

        .skills {
            display: grid;
            gap: 1rem;
        }

        .skill {
            display: flex;
            align-items: center;
        }

        .skill-name {
            width: 8rem;
            font-weight: 600;
            display: flex;
            align-items: center;
        }

        .skill-name i {
            margin-right: 0.5rem;
        }

        .skill-bar {
            flex-grow: 1;
            height: 1rem;
            background-color: var(--muted);
            border-radius: 0.5rem;
            overflow: hidden;
        }

        .skill-level {
            height: 100%;
            background-color: var(--primary);
        }

        .skill-percentage {
            width: 3rem;
            text-align: right;
        }

        .frameworks, .tools, .databases {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .tag {
            background-color: var(--primary);
            color: var(--primary-foreground);
            padding: 0.25rem 0.75rem;
            border-radius: 9999px;
            font-size: 0.875rem;
            font-weight: 500;
            display: flex;
            align-items: center;
        }

        .tag i {
            margin-right: 0.5rem;
        }

        .contact-links {
            display: grid;
            gap: 1rem;
        }

        .contact-link {
            display: flex;
            align-items: center;
            color: var(--foreground);
            text-decoration: none;
        }

        .contact-link i {
            margin-right: 0.5rem;
        }

        .blog-posts, .projects {
            display: grid;
            gap: 1rem;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        }

        .blog-post, .project {
            background-color: var(--muted);
            border-radius: 0.5rem;
            overflow: hidden;
        }

        .blog-post img, .project img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        .blog-post-content, .project-content {
            padding: 1rem;
        }

        @media (max-width: 640px) {
            header {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }

            .logo {
                margin-top: 1rem;
            }

            .skill {
                flex-direction: column;
                align-items: flex-start;
            }

            .skill-name {
                width: 100%;
                margin-bottom: 0.5rem;
            }

            .skill-percentage {
                width: 100%;
                text-align: left;
                margin-top: 0.25rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Paul Andrei Vicente</h1>
            <img src="logo.jpg" alt="Logo" class="logo">
        </header>

        <section class="section">
            <h2>About Me</h2>
            <p>Hi! I’m Paul Andrei Vicente , a passionate front-end enthusiast who loves music and design. 
                I’m constantly exploring new ways to blend creativity with code, bringing fresh ideas to life on screen.
                When I'm not practicing HTML, CSS, and JavaScript, I’m likely jamming out to my favorite tunes or 
                sketching new design concepts. This blog is a space to share my journey in web development, creativity, 
                and everything that inspires me along the way. Thanks for stopping by!</p>
        </section>

        <section class="section">
            <h2>Skills</h2>
            <div class="skills">
                <div class="skill">
                    <span class="skill-name"><i data-lucide="code"></i> HTML</span>
                    <div class="skill-bar">
                        <div class="skill-level" style="width: 70%;"></div>
                    </div>
                    <span class="skill-percentage">70%</span>
                </div>
                <div class="skill">
                    <span class="skill-name"><i data-lucide="palette"></i> CSS</span>
                    <div class="skill-bar">
                        <div class="skill-level" style="width: 80%;"></div>
                    </div>
                    <span class="skill-percentage">80%</span>
                </div>
                <div class="skill">
                    <span class="skill-name"><i data-lucide="file-code"></i> PHP</span>
                    <div class="skill-bar">
                        <div class="skill-level" style="width: 20%;"></div>
                    </div>
                    <span class="skill-percentage">20%</span>
                </div>
                <div class="skill">
                    <span class="skill-name"><i data-lucide="layout"></i> Bootstrap</span>
                    <div class="skill-bar">
                        <div class="skill-level" style="width: 30%;"></div>
                    </div>
                    <span class="skill-percentage">30%</span>
                </div>
                <div class="skill">
                    <span class="skill-name"><i data-lucide="layout"></i> Web Designing</span>
                    <div class="skill-bar">
                        <div class="skill-level" style="width: 80%;"></div>
                    </div>
                    <span class="skill-percentage">80%</span>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>Frameworks</h2>
            <div class="frameworks">
                <span class="tag"><i data-lucide="layout"></i> Bootstrap</span>
            </div>
        </section>

        <section class="section">
            <h2>Tools</h2>
            <div class="tools">
                <span class="tag"><i data-lucide="github"></i> GitHub</span>
            </div>
        </section>

        <section class="section">
            <h2>Databases</h2>
            <div class="databases">
                <span class="tag"><i data-lucide="database"></i> MySQL</span>
                <span class="tag"><i data-lucide="database"></i> MongoDB</span>
            </div>
        </section>

        <section class="section">
            <h2>Projects</h2>
            <div class="projects">
                <div class="project">
                    <img src="/placeholder.svg?height=150&width=250" alt="Project 1">
                    <div class="project-content">
                        <h3>Project 1</h3>
                        <p>Short description of Project 1</p>
                    </div>
                </div>
                <div class="project">
                    <img src="/placeholder.svg?height=150&width=250" alt="Project 2">
                    <div class="project-content">
                        <h3>Project 2</h3>
                        <p>Short description of Project 2</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>Blog</h2>
            <div class="blog-posts">
                <div class="blog-post">
                    <div class="blog-post-content">
                        <p>My love for music fuels my creativity in front-end design. Just like a song, 
                            a well-built website needs rhythm and balance—every line of code and design 
                            choice working together to create a seamless experience. 
                            I’m constantly practicing HTML, CSS, and JavaScript to bring my ideas to life on screen. 
                            The journey has its challenges, but it’s always worth it! </p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>Contact me</h2>
            <div class="contact-links">
                <a href="paulandreivicente.email@example.com" class="contact-link">
                    <i data-lucide="mail"></i> paulandreivicente.email@example.com
                </a>
                <a href="https://github.com/PaulAV-aghanimsSCEPTER" class="contact-link">
                    <i data-lucide="github"></i> https://github.com/PaulAV-aghanimsSCEPTER
                </a>
                <a href="https://www.facebook.com/stygian.d3solator26/" class="contact-link">
                    <i data-lucide="facebook"></i> https://www.facebook.com/stygian.d3solator26/
                </a>
            </div>
        </section>
    </div>

    <script>
        lucide.createIcons();
    </script>
</body>
</html>
