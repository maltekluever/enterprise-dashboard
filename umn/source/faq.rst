FAQ
===

Question: How can I filter the data for a specific timespan in a dashboard?
---------------------------------------------------------------------------

At the top right of each dashboard you find a dropbox with a clock icon where you can set the desired timespan as illustrated in the screenshot below:

.. image:: media/image27.png


Question: How can I create my own dashboard?
--------------------------------------------
In order to create a new custom dashboard, you click in the left menu on the dashboards-icon and click on "Create Dashboard" as illustrated below:

.. image:: media/image34.png

In the next step you can add panels and rows to the new dashboard. For comprehensive documentation please refer to the following Grafana docs:

Getting started: https://grafana.com/docs/guides/getting_started/
New Graphs in dashboards: https://grafana.com/docs/features/panels/graph/
New Tables in dashboards: https://grafana.com/docs/features/panels/table_panel/


Question: My panel is very crowded. How can I select only one category?
-----------------------------------------------------------------------

By default the consumption view shows all categories which sometimes make the graphs slightly overcrowded. In order to visualise only one specific category, you need to click on the desired category on the right side of the panel.

As an example, a click on "Compute" on the right side of Figure 1 will lead to a visualisiation of only this "Compute"-service as demonstrated in Figure 2.

.. image:: media/image28.png

Fig. 1: A panel visualising all categories

.. image:: media/image29.png
Fig. 2: A panel visualising only the category "compute"


Question: Can I use the Dashboard when data is updated?
-------------------------------------------------------

Yes, the dashboard will be accessible and data available.


Question: How can I download data?
----------------------------------

If you are an Editor or Admin User, it’s possible to download data
from each widget by clicking on the name of the widget Inspect
Data. You can then download the csv file. Additionally, data can be
received via API, please check chapter 4 API

.. image:: media/image30.png

Question: Where do I reset my password?
---------------------------------------

Please use this link

  https://enterprise-dashboard.otc-service.com/user/password/send-reset-email

Additionally, you can reset your password by following the “Forget
Password” link on the login page of Enterprise Dashboard.


Question: I can’t log in. What’s wrong?
---------------------------------------

You can use both email and username to login, but be aware that both
the log-in and forget password fields are case-sensitive. This means
if your email address is for example configured as Test@provider.com,
you also need to log in to Test@provider.com. test@provider.com will
not be recognized. If you forgot your password, use the link in
chapter 5.6. You can also change your email address to all minor case
within the preferences.


Question: I see users who are not added by me in the Grafana User management. Why?
----------------------------------------------------------------------------------

There are four default users which are used by operations or dashboard
squad itself to establish hotfixes or to help with customer issues.

- Admin

- Provisioning

- Account for Payer Dashboard

- Account for Tenant Dashboard


Question: I see “Average” and “Total” in almost every panel. How is this calculated?
------------------------------------------------------------------------------------

The average and total are calculated on the exact amount of datasets
in the selected timespan. More information here:

  https://grafana.com/docs/features/panels/graph/

Question: I can see some products with a cost of 0€ and some with 0.00€. What's the difference?
-----------------------------------------------------------------------------------------------

Products that have been used but are still in the free budget will be
displayed as 0€. 0.00€ will be displayed if there are costs smaller
than 1 cent. Technically those are still costs that will be invoiced,
therefore they are displayed in Enterprise Dashboard. You can hide
these products by ticking “hide series” options in the legend options
of each panel. Please note that editing a dashboard or panel is only
available for Editor or Admin Users.

.. image:: media/image31.png

Question: How do you handle daylight savings time changeover?
-------------------------------------------------------------

Within Enterprise Dashboard a changeover between summer and winter
time is visible on the specific dates by observing the quantity
field. For example, a machine that is never stopped will have a
runtime of 23 hours on the 28\ :sup:`th` of March 2021 and 25 hours on
the 27\ :sup:`th` of October 2019.

Below you will find the runtime of a unique machine, which was running
24/7. You can clearly see the drop on a S/W time changeover.

.. image:: media/image32.png

.. image:: media/image33.png

Question: Which version of Enterprise Dashboard do I have?
----------------------------------------------------------

Enterprise Dashboard will be listed within your invoice, therefore you
can see Enterprise Dashboard within your consumption data. Enterprise
Dashboard is billed on the first day of a month.

Question: I can not edit a query anymore. How can i solve this?
---------------------------------------------------------------

In the current grafana version is a bug which prevents you from
editing the query. You can select the the datasource and then 
the edior should appear again. (see the screenshot below)

.. image:: media/query-editor-failure.PNG
