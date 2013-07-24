Virginia Reporting Bundle

Author: Matt Walters

3rd Party Packages: Datatables jQuery plugin. http://datatables.net


Description: A number of reports to support virginia state reporting.


Current Report List:

Name: Log Entry Search
Description: Allows searching of log entries by Virginia state information.

Name: Truancy Counts
Description: Mimics the truancy count table found on the VA SRC verification report.

Name: Count of Disability Types
Description: Mimics the student disability count table found on the VA SRC.

Name: Count of LEP students by ESL codes
Description: Mimics the LEP student count table found on the VA SRC.

Name: Roster Detail
Description: Attempts to mimic the MSC roster detail report.

Name: MSC Section Search
Description: Allows searching of sections for MSC data by commonly used IDs in the DOE error reports.


Installation:

Custom Web Root: Copy the admin, images, and scripts folder into the custom web_root.

CPM Import: Import cpm_import.zip. Manually upload the image and SWF files located in:
/images/css/vrb/custom-theme/images/*
/images/vrb/*
/scripts/vrb/DataTables/images/*
/scripts/vrb/DataTables/extras/TableTools/images/*
/scripts/vrb/DataTables/extras/TableTools/swf/*

Edit /admin/reports/reporttabs.html and add the following lines between a
</li> and a <li> or between a </li> and </ul> to add the VRB tab to the reports page.

<!-- Begin VRB Link -->
<li class="~[if.~[gpv:repType]=vrb]selected[/if]">
    <a href="~[if.~[gpv:repType]=vrb]#[else]/admin/reports/vrb/home.html[/if]">VRB</a>
</li>
<!-- End VRB Link -->


History:
---------- 07/24/2013 ----------
Fixed a couple images paths.
Added MSC Section Search report.

---------- 07/23/2013 ----------
First "proper" master branch commit. 