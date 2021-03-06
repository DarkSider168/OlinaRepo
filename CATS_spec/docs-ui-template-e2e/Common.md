# Common

These test cases covered hub page,conceptual page,reference namespace page and reference class type page and total 6 cases currently.Every test case includes check point, steps and expected behavior.

**Below is test cases list:**
* [Verify all links of Header and Footer](#Verify_all_links_of_Header_and_Footer)
* [Verify themeSelector](#Verify_themeSelector)
* [Verify sharing button](#Verify_sharing_button)
* [Breadcrumb validation](#Breadcrumb_validation)
* [Verify Toc is presented and links are able to click](#Verify_Toc_is_presented_and_links_are_able_to_click)
* [Verify RedirectUrl work well](#Verify_RedirectUrl_work_well)

## <a id='Verify_all_links_of_Header_and_Footer'></a>Verify all links of Header and Footer
### Check point
* Verify the footer Privacy Statement is existed and the link is expected
* Verify the footer Term Of Use is existed and the link is expected
* Verify the footer Feedback is existed and the link is expected
* Verify the footer Trademarks is existed and the link is expected
* Verify the sequence of these 4 items is accurate

**Steps**
1. Open a sample page
2. Find corresponding link elements 
3. Find corresponding link elements

**Expected behavior**
* These 4 items all reveal on page
* The sequence of these 4 items is accurate on page
* The value of attribute 'href' and expected are consistent for these 4 items

## <a id='Verify_themeSelector'></a>Verify themeSelector
### Check point
* Verify the Theme Selector are shown and can be clicked
* Verify the element: html contain theme_night class when choose dark theme, and non for light theme

**Steps**
1. Open a sample page
2. Find component Theme selector
3. Switch to 'Dark' theme 
4. Check if the class value contains 'theme_night'
5. Switch to 'Light' theme
6. Check if the class value is non

**Expected behavior**
* The Theme Selector are shown and can be clicked
* The theme 'Light' and 'Dark' are reveal
* The theme class value is expected

## <a id='Verify_sharing_button'></a>Verify sharing button
### Check point
* Verify the Sharing button is present
* Verify the Sharing Facebook and Twitter is presented
* Verify the Sharing button can be clicked
* Verify the links of Sharing Facebook and Twitter  is accurate

**Steps**
1. Open a sample conceptual page
2. Find 'Share' button
3. Click the 'Share' button
4. Check element 'Facebook'
5. Check value the attribute 'href' of Facebook link

**Expected behavior**
* The Sharing button is present
* The Sharing button can be clicked
* The Sharing Facebook is presented
* The links of Sharing Facebook is accurate

## <a id='Breadcrumb_validation'></a>Breadcrumb validation
### Check point
* Verify the Breadcrumb is presented on conceptual page

**Steps**
1. Open a sample page
2. Find breadcrumb element on conceptual page
3. Verify the count of breadcrumb element

**Expected behavior**
* The breadcrumb element count is greater than 0

## <a id='Verify_Toc_is_presented_and_links_are_able_to_click'></a>Verify Toc is presented and links are able to click
### Check point
*Reference*
* Verify the TOC List is presented
* Verify the TOC list header is expected

*Conceptual*
* Verify the TOC List is shown
* Verify the particular TOC links to an expected URL

**Steps**
1. Open a sample page
2. Find the TOC items
3. Check the TOC items if presented
4. Click another sample TOC item at the same level
5. Check if redirect to expected page
6. Check the TOC header name if expected

**Expected behavior**
* TOC list is presented
* TOC item at the same level is able to click
* The url of page switch to is expected
* The TOC header items name is expected

## <a id='Verify_RedirectUrl_work_well'></a>Verify RedirectUrl work well
### Check point
* Verify page will go to the assigned page

**Steps**
1. Open a sample page
2. Verify page will go to the assigned page <URL_InstallATA_Conceptual>
3. Verify page will go to the 404 page as invalidAbsoluteUrl
4. Verify page will go to the 404 page as emptyRelativeUrl
5. Verify page will go to the 404 page as invalidRelativeUrl
6. Verify page will go to the RelativePage page

**Expected behavior**
* The value of test page url and expected are consistent
* The page is able to go to assigned 404 page
