# Data For A Cause: DonorsChoose.org

This week I participated in [Data for a Cause](http://www.olgatsubiks.com/data-for-a-cause), a weekly competition where data geeks can access a dataset from a non-profit and submit data visualizations to acheive a particular goal. 

This week the non-profit is [DonorsChoose.org](https://www.donorschoose.org/?utm_source=Data+for+a+cause+challenge&utm_campaign=1bd1a1722d-Data_for_a_cause_Start_2_20_2017&utm_medium=email&utm_term=0_8d5c6df296-1bd1a1722d-165586173), an organization that empowers public school teachers from the United States to request much-needed materials and experiences for their students. DonorsChoose.org submitted a [rich dataset](https://gallery.mailchimp.com/ee9380403e469486e9da3ef97/files/77da6d68-7a94-466c-878b-c0564cd0390b/DonorsChoose.org_Data_Layout.pdf?utm_source=Data+for+a+cause+challenge&utm_campaign=1bd1a1722d-Data_for_a_cause_Start_2_20_2017&utm_medium=email&utm_term=0_8d5c6df296-1bd1a1722d-165586173) covering donations, recipients, and requests.

*The goal:* create a data visualization aimed at policy makers to show the inequality of the public school system.
*The audience:* policy makers and education leaders.


First I downloaded the data and entered it into SQLServer.

```sql
CREATE Table DonorsChooseRaw (

_projectid varchar(200)
,_teacher_acctid varchar(200)
,_schoolid varchar(200)
,school_ncesid varchar(200)
,school_latitude varchar(200)
,school_longitude varchar(200)
,school_city varchar(200)
,school_state varchar(200)
,school_zip varchar(200)
,school_metro varchar(200)
,school_district varchar(200)
,school_county varchar(200)
,school_charter varchar(200)
,school_magnet varchar(200)
,school_year_round varchar(200)
,school_nlns varchar(200)
,school_kipp varchar(200)
,school_charter_ready_promise varchar(200)
,teacher_prefix varchar(200)
,teacher_teach_for_america varchar(200)
,teacher_ny_teaching_fellow varchar(200)
,primary_focus_subject varchar(200)
,primary_focus_area varchar(200)
,secondary_focus_subject varchar(200)
,secondary_focus_area varchar(200)
,resource_type varchar(200)
,poverty_level varchar(200)
,grade_level varchar(200)
,vendor_shipping_charges varchar(200)
,sales_tax varchar(200)
,payment_processing_charges varchar(200)
,fulfillment_labor_materials varchar(200)
,total_price_excluding_optional_support varchar(200)
,total_price_including_optional_support varchar(200)
,students_reached varchar(200)
,total_donations varchar(200)
,num_donors varchar(200)
,eligible_double_your_impact_match varchar(200)
,eligible_almost_home_match varchar(200)
,funding_status varchar(200)
,date_posted varchar(200)
,date_completed varchar(200)
,date_thank_you_packet_mailed varchar(200)
,date_expiration varchar(200))
```




What are teachers asking for?

What do donors think is worth supporting?