<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
  TBD-step-1-notes.
-->

## Step 1: Create a Quarto doc

_Welcome to "Share Great Tables with Quarto and Cloud Connect"! :wave:_

Our first step is to make a Quarto document to put our table in.

**What is a Quarto?**: A Quarto document (.qmd) is a plain-text markdown file that contains 
code chunks written in Python, R, Julia, or Observable. When you render the document, Quarto formats the markdown into a polished report and inserts the output of the code chunks.

Read more about Quarto at [quarto.org](https://quarto.org/). 

### :keyboard: Activity: Make a quarto document

1. Open a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
  
2. On the < > Code tab in the header menu of your repository, select the **Add file** drop-down and click **Create new file**.

   ![create new file option](/images/create-new-file.png)

3. In the **Name your file...** field, enter `table.qmd`.

4. In the **Enter file contents here** area, copy the following content to your file:

   ```
   ---
   title: "Check this out..."
   format: html
   jupyter: python3
   ---
   
   ```

   ![profile.md file screenshot](/images/my-quarto-file.png)

   Quarto files begin with a YAML header that contains metadata used to render the file. This header begins an empty Quarto doc that can be rendered to HTML and contain executable python chunks.

6. Click **Commit changes...** in the upper right corner above the contents box. 

   ![screenshot of adding a new file with a commit message](/images/commit-top-of-page.png)

7. Then click **Commit changes** in the pop up window that appears.

   ![screenshot of adding a new file with a commit message](/images/commit-full-screen.png)
   
8. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
