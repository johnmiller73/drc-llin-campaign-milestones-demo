# Progress data

Put the CSV exported from the milestone update sheet here as **`milestone_status.csv`**.

- If this file is missing, the dashboard shows demonstration data and the "DEMONSTRATION DATA" banner.
- Once it's here, the dashboard reads statuses from it and the banner changes to "PROGRESS DATA".

The dashboard finds columns by their headings. It needs `Province`, `Milestone ID` and `Status`. It also uses `Planned due date`, `Actual completion date`, `Notes`, `Milestone`, `Stage` and `Region` if they're there. Don't rename the headings in the sheet.
