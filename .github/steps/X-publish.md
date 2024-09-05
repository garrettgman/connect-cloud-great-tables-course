<!--
  <<< Author notes: Step 4 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-4-notes.
-->

## Step 4: Publish

_Almost there! :heart:_

Let's publish that table to Posit Cloud Connect!

**What is _Posit Connect Cloud_**: Posit Connect Cloud is a cloud environment to easily showcase your Python and R content. You authenticate into GitHub from Posit Connect Cloud and then publish R or Python backed content straight from your repos to the web. Learn more [here](https://connect.posit.cloud/).

### :keyboard: Activity: Publish table to Posit Connect Cloud

1. In a new tab, **visit** <https://connect.posit.cloud/>

2. **Click Sign Up**

   <img src="/images/click-sign-up.png" width="600"/>

3. **Click Sign In with GitHub**. Follow the steps to **authenticate to your GitHub account**. We want to prove it is you!

   <img src="/images/sign-in-with-github.png" width="300"/>

4. From your Connect Cloud home screen, **click Publish.**

   <img src="/images/publish.png" width="600"/>

5. **Select Quarto** as your framework, because you are publishing a Quarto doc.

   <img src="/images/framework.png" width="500"/>

6. **Select your `connect-cloud-great-tables-course` repo.** This is the repo that has the file you want to publish.

   <img src="/images/repo.png" width="500"/>

7. **Select the `main` branch.** This is the branch of the repo that has the file you want to publish.

   <img src="/images/branch.png" width="500"/>

8. **Select `table.qmd`.** This is the file you want to publish.

   <img src="/images/file.png" width="500"/>

9. **Click Publish**.

   <img src="/images/publish-2.png" width="500"/>

10. Wait a minute or less. Posit Connect Cloud will quickly:

    1. Clone your repo
    2. Create a Python environment to render your Quarto doc in
    3. Render the doc
    4. Publish the result 

   <img src="/images/process.png" width="600"/>

11. **Ta da!** You should be looking at your published content, and it should look like this.

   <img src="/images/published-table.png" width="600"/>

## Recap
  
_Congratulations friend, you've completed this course!_

Here's a recap of all the tasks you've accomplished in your repository:

- Made a Quarto doc
- Added a Python code chunk that generates a great table
- Added a requirements.txt file
- Published the Quarto doc to Posit Connect Cloud


## Share and Maintain your table

Now that your table is on Posit Connect Cloud, you can

1. **Share the table.** Click the Share icon to copy the URL associated with the table. Anyone can visit your table at this URL.

   <img src="/images/share.png" width=600>

3. **Republish the table**. To do so, click the republish button in the sidebar.

   <img src="/images/republish.png" width=600>

   Republishing will scoop up any changes you've made on GitHub. Posit Connect Cloud will eventually scoop up these changes on its own, but republishing the app makes it happen immediately.

4. You can find these features, and more, next to your app on your Posit Connect home page.

   <img src="/images/portfolio.png" width=600>

### What's next?

- [Learn more about Posit Connect Cloud](https://docs.posit.co/connect-cloud/how-to/)
- [Expand your Great Tables acumen](https://posit-dev.github.io/great-tables/articles/intro.html)
- [Use Quarto to make code-powered dashboards, pdfs, and so much more](https://quarto.org/)

