Hello, since I unfortunately don't know how to do it with github, I'll do it like this


Html : 

<!DOCTYPE html>
<html>
    <head>
    <title>Led Button</title>
    <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <a href="#" style="--clr:#E43607">Button</a>
        <a href="#" style="--clr:#07ABE4">Button</a>
        <a href="#" style="--clr:#E4E407">Button</a>
    </body>
</html>

Css:
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
body
{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    flex-direction: column;
    gap: 40px;
    background: #393835;
}
a
{
    position: relative;
    background: #686764;
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 1.5em;
    letter-spacing: 0.1em;
    font-weight: 400;
    padding: 10px 30px;
    transition: 0.5s;
}
a:hover
{
    letter-spacing: 0.25em;
    background: var(--clr);
    box-shadow: 0 0 35px var(--clr);
}
a::before
{
    content: '';
    position: absolute;
    inset: 2px;
}
a span
{
    position: relative;
    z-index: 1;
}
