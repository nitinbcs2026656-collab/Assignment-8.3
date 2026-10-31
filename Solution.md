```html
<!DOCTYPE html>
<html>
<head>
    <title>Magazine Layout</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }

        .container {
            display: grid;
            grid-template-columns: 2fr 1fr;
            grid-template-areas:
                "header header"
                "nav nav"
                "article sidebar"
                "footer footer";
            gap: 10px;
            padding: 10px;
        }

        header {
            grid-area: header;
            background: #1e293b;
            color: white;
            padding: 20px;
        }

        nav {
            grid-area: nav;
            background: #64748b;
            color: white;
            padding: 15px;
        }

        article {
            grid-area: article;
            background: #e2e8f0;
            padding: 20px;
        }

        aside {
            grid-area: sidebar;
            background: #cbd5e1;
            padding: 20px;
        }

        footer {
            grid-area: footer;
            background: #1e293b;
            color: white;
            text-align: center;
            padding: 15px;
        }

        @media (max-width: 600px) {
            .container {
                grid-template-columns: 1fr;
                grid-template-areas:
                    "header"
                    "nav"
                    "article"
                    "sidebar"
                    "footer";
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header><h1>Daily Magazine</h1></header>
        <nav>Home | News | Technology | Sports</nav>

        <article>
            <h2>Main Article</h2>
            <p>Technology is changing our world. New innovations make life easier and more connected.</p>
        </article>

        <aside>
            <h3>Latest News</h3>
            <p>Education Updates</p>
            <p>Technology News</p>
            <p>Sports Headlines</p>
        </aside>

        <footer>© 2026 Daily Magazine</footer>
    </div>
</body>
</html>
```