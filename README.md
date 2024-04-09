   https://www.freecodecamp.org/news/how-to-deploy-next-js-app-to-github-pages/
   
   action.yml
    It declares a composite action. The composite action allows you to bundle multiple workflow steps into a single action, combining multiple run commands into a single reusable action.
    It creates a new build environment and sets up Node.js 20 there.
    It installs npm dependencies and uses a caching mechanism to speed up this process.



    publish.yml
        This action is executed when code is pushed or merged into the main branch.
    It uses the setup-node action to set up the environment.
    The action has two stages: in the first stage, the Next.js app is bundled. In the second stage, we upload the artifacts from the first stage to GitHub Pages.