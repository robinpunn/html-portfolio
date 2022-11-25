****

<h1 style="color:purple;">EMAIL DEVELOPMENT PORTFOLIO</h1>

****

<h3 style="color:purple";> This project was created with <a href="https://getbootstrap.com/docs/5.2/getting-started/introduction/" target="_blank">Bootstrap</a> and bundled with <a href="https://parceljs.org/docs/" target="_blank">Parcel</a> </h3>

****

<h4 style="color:purple"> Installed Boostrap and Parcel with npm </h4>

```npm install bootstrap@5.2.3 ```

```npm i --save-dev parcel ```

<h4 style="color:purple"> I was having trouble hosting on github but was sucessful following the steps below </h4>

<h6 style="color:purple"> I first moved all my files from 'pages' into the 'src' folder so that they were in the same path with index.html (this may not be necessary) </h6>

1. <p style="color:purple">Create a "gh-pages" branch</p>

    ``` git branch gh-pages ```

2. <p style="color:purple">Switch to gh-pages branch</p>

    ``` git checkout gh-pages ```

3. <p style="color:purple"><a href="https://stackoverflow.com/questions/20101994/how-to-git-pull-from-master-into-the-development-branch/20103414#20103414" target="_blank">Fetch</a> from main branch.</p>

    ``` git fetch origin ```

4. <p style="color:purple">Added these scripts to package.json:</p>

    ```"build": "parcel build src/index.html", ```
    ```"predeploy": "rm -rf dist && parcel build src/index.html src/about.html src/skills.html src/portfolio.html --public-url ./", ```
    ```"deploy": "gh-pages -d dist" ```

5. <p style="color:purple">Run the predeploy and deploy commands</p>

    ``` npm run predeploy ```
    ``` npm run deploy ```

6. <p style="color:purple">In the github reposirtory settings/pages section, make sure the gh-branches section is selected.</p>