<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-2-notes.
-->

## Step 2: Add a great table

_You made a Quarto document! :tada:_

Now let's add a great table to your Quarto doc.

**What is a _great table?_**: A great table is a polars or pandas dataframe polished for publication with the Great Tables package. Great Tables lets you mix and match things like headers, footers, row stubs, column spanners, labels, and much more. Not only that, you can format the cells in a variety of awesome ways.

Read more about the Great Tables package [here](https://posit-dev.github.io/great-tables/articles/intro.html). 

### :keyboard: Activity: Add a table to your Quarto doc

1. Open `table.qmd`.
    
3. Click on the **pencil icon** to edit the contents of `table.qmd`.

   <img src="/images/edit.png" width="500"/>

5. Add the following content to the bottom of the file.

   ````
 
   ```{python}
   #| echo: false
   
   ```
   ````

   This creates a Python code chunk. Now we can add any Python code you like between the chunk fences (```). When you render the document, Quarto will run the code and append its results into a polished HTML file. `#| echo: false` tells Quarto to include the results of the code chunk, but not the code itself.

6. Under `#| echo: false` add code that creates a great table. Don't have one handy? Use this code. When run, it makes the table below.

   <img src="/images/solar-table.png" width="600"/>

   ```
   from great_tables import GT, html
   from great_tables.data import sza
   import polars as pl
   import polars.selectors as cs
   
   sza_pivot = (
       pl.from_pandas(sza)
       .filter((pl.col("latitude") == "20") & (pl.col("tst") <= "1200"))
       .select(pl.col("*").exclude("latitude"))
       .drop_nulls()
       .pivot(values="sza", index="month", on="tst", sort_columns=True)
   )
   
   (
       GT(sza_pivot, rowname_col="month")
       .data_color(
           domain=[90, 0],
           palette=["rebeccapurple", "white", "orange"],
           na_color="white",
       )
       .tab_header(
           title="Solar Zenith Angles from 05:30 to 12:00",
           subtitle=html("Average monthly values at latitude of 20&deg;N."),
       )
       .sub_missing(missing_text="")
   )
   ```

   Your file should now look something like this. If you'd like to add a text introduction for your table, you can write it above the Python code chunk.
   
   <img src="/images/table-on-github.png" width="600"/>

8. Click **Commit changes...** in the upper right corner above the contents box to save your changes.

   <img src="/images/commit-top-of-page.png" width="600"/>

9. Then click **Commit changes** in the pop up window that appears.

   <img src="/images/commit-full-screen-2.png" width="400"/>

   
10. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
