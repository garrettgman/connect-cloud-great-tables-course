<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-3-notes.
-->

## Step 3: Add a requirements.txt file

_Nice work finishing your Python chunk! :sparkles:_

Now, when someone renders your Quarto doc, it will emit an HTML report that looks like this.

<img src="/images/finished-report.png" width="600"/>

You could render the report yourself, locally. See how [here](https://quarto.org/docs/get-started/authoring/vscode.html#rendering). But we are going to publish this repository to Posit Connect Cloud. Posit Connect Cloud will render the report for you in the cloud and display the results at a URL. 

To do that, Posit Connect Cloud will need to set up a Python environment that can run your code. You can tell Posit Connect Cloud which packages to install by creating a `requirements.txt` file. 

**What is a `requirements.txt` file**: By convention, when Python users share a project, they include a file named `requirements.txt` that lists the names of the packages used by the project. Other Python users can quickly install these packages with a command like:

```
pip install -r /path/to/requirements.txt
```

### :keyboard: Activity: Add a `requirements.txt` file

1. On the < > Code tab in the header menu of your repository, select the **Add file** drop-down and click **Create new file**.

   <img src="/images/create-new-file.png" width="400"/>

3. In the **Name your file...** field, enter `requirements.txt`.

4. In the **Enter file contents here** area, copy the following content to your file:

   ```
   great_tables
   jupyter
   pandas
   polars
   quarto
   ```

   <img src="/images/requirements.png" width="600"/>

   These are the packages needed to run your code chunk. Add additional package names as necessary if you supplied your own code to build the table.

6. Click **Commit changes...** in the upper right corner above the contents box.

   <img src="/images/commit-top-of-page-3.png" width="600"/>

7. Then click **Commit changes** in the pop up window that appears.

   <img src="/images/commit-full-screen-3.png" width="400"/>
   
8. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
