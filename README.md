# Community Workshop Attendance Visualization

## Visualization question and audience

**Question:** How does community workshop attendance vary across
neighborhoods?

**Intended audience:** Community program administrators and local
government officials who use attendance information to understand
participation and support program and resource-planning decisions.

The visualization compares the number of workshop visits across
neighborhoods for the selected month. It is intended as a clear,
month-specific view of attendance---not as a measure of utilization or
proof of why attendance differs.

## Data source and reuse

The project uses the course-provided community workshop dataset, saved
as `tableau_workshops_tidy.csv`.

-   **Data status:** Simulated data created for educational/coursework
    purposes. These values are not actual observations of community
    programs.
-   **Attribution:** Retain the original course/source attribution
    supplied with the dataset when copying, sharing, or publishing the
    data. **Add the exact source/creator attribution here:**
    `[Insert the attribution exactly as provided with the course dataset.]`
-   **Reuse:** Use the dataset in accordance with the course/source
    terms. Do not present simulated values as real-world findings or
    imply that they describe actual neighborhoods or program
    participants.
-   **Publishing:** Only publish the simulated course data and project
    materials permitted by the course/source terms.

## Project files

The files below are included in the Module 1/Module 2 working outputs.

  -----------------------------------------------------------------------
  Filename                            Contents
  ----------------------------------- -----------------------------------
  `tableau_workshops_tidy.csv`        Tidy workshop dataset used in
                                      Tableau and Python.

  `m01_claim_check.csv`               Python claim-check values used to
                                      verify the selected Tableau chart.

  `m01_after_chart.png`               Reference image of the
                                      selected/updated Module 1 chart.

  `m01_before_after.png`              Before-and-after visualization
                                      evidence.

  `module_2_file_guide.txt`           Notes identifying the selected
                                      chart month and the purpose of the
                                      project files.

  `run_record.json`                   Run or execution record associated
                                      with the saved outputs.

  `m01_graduate_check.csv`            Supporting numerical check for the
                                      graduate-level extension.

  `m01_graduate_missingness.png`      Supporting visualization of the
                                      missing-data analysis.
  -----------------------------------------------------------------------

## Run the Module 1 notebook in Google Colab

1.  Open the personal Module 1 notebook using this link: **\[Insert your
    working Colab notebook URL\]**.
2.  Sign in to Google if prompted.
3.  Upload the project input file(s) when the notebook requests them, or
    make sure they are available in the notebook's expected location.
4.  In Colab, select **Runtime → Run all** to execute the notebook from
    top to bottom.
5.  Review the output cells for the chart and validation results.
6.  The saved project files are located in the Colab folder
    `/content/outputs/`. In the Colab Files pane, open the `outputs`
    folder to view or download them.

If the notebook uses Google Drive rather than a direct upload, mount
Drive when prompted and follow the notebook's existing file-path
instructions.

## Selected chart and Tableau settings

-   **Selected chart month:** October 2026.
-   **Data source:** `tableau_workshops_tidy.csv`.
-   **Month filter:** Keep only October 2026 (`2026-10-01`).
-   **Rows:** `Neighborhood`.
-   **Columns:** `SUM(Attendance Visits)`.
-   **Marks:** Horizontal bars, with attendance values displayed as
    labels.
-   **Units:** Number of attendance visits (counts), not percentages.
-   **Aggregation:** Sum of attendance visits for each neighborhood in
    October 2026. The month filter leaves one monthly record per
    neighborhood, so each neighborhood is represented by one bar.
-   **Axis:** Start the attendance axis at zero to support a fair visual
    comparison.

To match the reference chart, use the October 2026 filter and the sum of
attendance visits. Do not use the six-month utilization calculations for
this month-specific attendance chart.

## Expected checked values

The expected October 2026 attendance values are:

  Neighborhood     Expected attendance visits
  -------------- ----------------------------
  East                                     94
  West                                     90
  North                                    90
  South                                    82

The chart order in the reference is East, West, North, South. North and
West have the same expected attendance value, so their relative order
does not change the numerical comparison.

Use `m01_claim_check.csv` as the Python claim-check reference and
compare its values with the values displayed in Tableau. The comparison
should show a difference of **0** for each neighborhood when the same
month, measure, and aggregation are used. The `m01_after_chart.png` file
provides visual evidence of the selected chart. `m01_before_after.png`,
`m01_graduate_check.csv`, and `m01_graduate_missingness.png` provide
additional supporting evidence for the broader visualization and
data-quality work.

**Validation note:** Before final submission, confirm that the `month`
field in `m01_claim_check.csv` is October 2026 and that its four values
match the table above. If the CSV contains a different month, regenerate
or correct the claim-check file from `tableau_workshops_tidy.csv` using
the October 2026 filter rather than treating a different month's values
as October results.

## Tableau workbook and access

-   **Workbook filename:**
    `[Insert the saved Tableau workbook filename, preferably the packaged .twbx file.]`
-   **Published Tableau view (if applicable):**
    `[Insert the working Tableau Public or Tableau Cloud view URL.]`
-   **Access instructions:** Open the workbook file in Tableau Desktop,
    or open the published view link in a browser. If the published view
    is private or requires sign-in, grant the instructor/viewers the
    required access before submission.

Include the workbook or a working view link with the submitted README so
the chart can be reviewed.

## Interpretation and limitation

The chart compares attendance counts for one month; it does not show
attendance relative to capacity. It also relies on simulated data, so
the results should be interpreted as a coursework demonstration rather
than evidence about actual community participation. Missing or
incomplete attendance records should be identified rather than
automatically interpreted as zero attendance.
