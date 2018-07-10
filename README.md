# sample-private-template-library

This template library exists for you to use as a basis for your own template library.

You should fork (or download and copy) this repository to initialise your own.

Smart Legal Contract Templates conform to the [Accord Project Template Specification](https://docs.google.com/document/d/1UacA_r2KGcBA2D4voDgGE8jqid-Uh4Dt09AE-shBKR0), the protocol is managed by the open-source community of the [Accord Project](https://accordproject.org). 

These templates can be parsed and executed by the [Cicero](https://github.com/accordproject/cicero) engine.

## Building and deploying

The `run.js` script in this project will generate static webpages, and template archives for each of the templates in the `src` folder.

1. After cloning your repository the following command to install all of the required tools

        npm install

2. All of your templates should pass their unit tests before you generate a template site

        npm run test

3. Then to build the archives and website, run:

        npm run build

4. Finally to publish your static site to [Netlify](https://netlify.com), you should authorise your command line to publish to your Netlify account. This step is only required once.

        npm run deploy:init
    
    Then, publish the build with

        npm run deploy

    Output
    ```
    mattmbp:sample-private-template-library matt$ npm run deploy

    > @clausehq/sample-private-template-library@0.1.0 deploy /Users/matt/dev/clauseHQ/sample-private-template-library
    > netlify deploy

    ? No site id specified, create a new site Yes
    Deploying folder: build

    Deploy is live (permalink):
    http://5b449604c6aed618d01630b4.xenodochial-meninsky-27f070.netlify.com

    Last build is always accessible on http://xenodochial-meninsky-27f070.netlify.com
    ```