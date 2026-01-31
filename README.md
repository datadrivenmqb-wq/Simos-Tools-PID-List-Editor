# Simos-Tools-PID-List-Editor
HTML-based PID List Editor for Simos Tools logging lists

Description:
This is a responsive PID List Editor for building and modifying Simos Tools logging lists. The purpose is to call out duplicate PIDs, show which are calculated, and allow easy combinining of multiple PID lists for customization. 

Download instructions: Click on the PID List Editor (html) file. Select "Download raw file" in the upper RH corner. When downloaded, simply open the html file and it will launch in your web browser.

How to use:
1. Select a base logging list to start with. This can be what you're using currently, or something that mostly fits your needs. All PIDs from this initial base list will be "activated" or checked by default. Green PIDs are native PIDs direct from the car, blue PIDs are calculated (based on having a 0xffff or 0xffffffff address, depending on whether it is a Mode 22 or HSL list).

2. Select a second logging list to add more PIDs. These additional logging list PIDs will be appended at the bottom and unchecked or "deactivated" by default. Note that this does not affect the "Enabled" column, but is merely for selecting which to combine into a list. Note that more than one additional logging list may be appended, this button can be used multiple times.

3. Edit the list for export. Yellow PIDs are those which are currently disabled and new from the secondary logging list(s), and may be checked to be added to the "final" list. Note that for Calculated PIDs (0xffff or 0xffffffff) instead of using the Address to determine as a duplicate, it uses the Name column. So two PID lists with a "Calc HP" and a "Calculated HP" PID which are otherwise identical will NOT be flagged as a duplicate. Red PIDs are active duplicates. Comparing and unchecking one of them will resolve the issue and prevent from having multiple PIDs doing the same thing. Note that all fields are editable for customization to formulas, warning limits, etc.

4. Hints for editing: You can use the various filters to find what is needed. Those filters include: PID type (buttons at top) and the search field. The search field is across ALL columns at once. When filtering, this does NOT activate or deactivate any PIDs, just hides some from view. You may also choose to sort by whichever column you like, with a secondary sorting also available if desired. Clicking "Reset" in the sort area will return to the original sort state (Primary PID list on top, any secondary PID lists at the bottom).

5. Export PID List: All activated (checked) PIDs are exported in the displayed order. Preview by filtering to only see Active and Calculated Active PIDs.
