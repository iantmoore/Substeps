---
title: Substeps | Webdriver | Step Implementations
layout: documentation
---

Webdriver Step Implementations
==============================

<table border="1">
<tr><th>Keyword</th> <th>Example</th> <th>Description</th></tr>
<tr><td colspan="3"><strong>Assertions</strong></td></tr>
<tr><td>AssertCheckBox checked=&quot;&lt;checkedString&gt;&quot;</td><td>AssertCheckBox checked=true/false</td><td>Check that the current element, a checkbox is checked or not</td></tr>
<tr><td>AssertCurrentElement attribute=&quot;&lt;attribute&gt;&quot; value=&quot;&lt;expected&gt;&quot;</td><td>AssertCurrentElement attribute="class" value="icon32x32"</td><td>Check that the current element has the specified attribute and value</td></tr>
<tr><td>AssertCurrentElement has attributes=[&lt;attributeString&gt;]</td><td>AssertCurrentElement has
          attributes=[type="submit",value="Search"]</td><td>Check that the current element has the specified attributes</td></tr>
<tr><td>AssertCurrentElement text contains &quot;&lt;expected&gt;&quot;</td><td>AssertCurrentElement text contains "Hello world"</td><td>Check that the current element contains the specified text</td></tr>
<tr><td>AssertCurrentElement text=&quot;&lt;expected&gt;&quot;</td><td>AssertCurrentElement text="Hello World!"</td><td>Check that the current element has the expected text value</td></tr>
<tr><td>AssertCurrentInput value=&quot;&lt;expected&gt;&quot;</td><td>AssertCurrentInput value="Hello World!"</td><td>Check that the current input field has the expected text value</td></tr>
<tr><td>AssertEventuallyContains &lt;elementId&gt; &quot;&lt;text&gt;&quot;</td><td>AssertEventuallyContains mySpanId "text I eventually expect"</td><td>Asserts that an element (identified by ID) eventually gets some specific  text inserted into it (by JavaScript, probably)</td></tr>
<tr><td>AssertNotPresent text=&quot;&lt;text&gt;&quot;</td><td>AssertNotPresent text="undesirable text"</td><td>Assert that the specified text is not found within the page</td></tr>
<tr><td>AssertPageTitle is &quot;&lt;expectedTitle&gt;&quot;</td><td>AssertPageTitle is "My Home Page"</td><td>Check that the page title is ....</td></tr>
<tr><td>AssertRadioButton checked=&quot;&lt;checkedString&gt;&quot;</td><td>AssertRadioButton checked=true/false</td><td>Check that the current element, a radio button, is checked or not</td></tr>
<tr><td>AssertTagElementContainsAttribute tag=&quot;&lt;tag&gt;&quot; attributeName=&quot;&lt;attributeName&gt;&quot; attributeValue=&quot;&lt;attributeValue&gt;&quot;</td><td>AssertTagElementContainsText tag="ul" attributeName="class"
          attributeValue="a_list"</td><td>Check that any of the html tags have the specified attribute name and  value</td></tr>
<tr><td colspan="3"><strong>Clicks</strong></td></tr>
<tr><td>Click</td><td>Click</td><td>Click (the current element)</td></tr>
<tr><td>ClickButton &lt;buttonText&gt;</td><td>ClickButton submit</td><td>Click a button that has the text...</td></tr>
<tr><td>ClickById &lt;id&gt;</td><td>ClickById login</td><td>Find an element by id, then click it.</td></tr>
<tr><td>ClickLink &quot;&lt;linkText&gt;&quot;</td><td>ClickLink "Contracts"</td><td>Click the link &quot;(....)&quot; as it appears on the page</td></tr>
<tr><td>PerformContextClick</td><td>PerformContextClick</td><td>Performs a context click (typically right click, unless this has been  changed by the user) on the current element.</td></tr>
<tr><td>PerformDoubleClick</td><td>PerformDoubleClick</td><td>Performs a double click on the current element (set with a previous Find  method).</td></tr>
<tr><td>Submit</td><td>Submit</td><td>Submit the form of the current element. NB using click is preferable as  javascript may be executed on click, which this method would bypass</td></tr>
<tr><td colspan="3"><strong>Forms</strong></td></tr>
<tr><td>AssertRadioButton name=&quot;&lt;name&gt;&quot;, text=&quot;&lt;text&gt;&quot;, checked=&quot;&lt;checked&gt;&quot;</td><td>AssertRadioButton name="radio_btn_name", text="text",
          checked="true"</td><td>Asserts a value of a radio button</td></tr>
<tr><td>ChooseOption &quot;&lt;value&gt;&quot; in current element</td><td>ChooseOption "fred" in current element</td><td>Select a value in the option list in the current element, a Find  operation is required immediatebly before</td></tr>
<tr><td>ChooseOption &quot;&lt;value&gt;&quot; in id &lt;id&gt;</td><td>ChooseOption "fred" in id usersList</td><td>Select a value in the option list that has the id</td></tr>
<tr><td>ClearAndSendKeys &quot;&lt;value&gt;&quot;</td><td>ClearAndSendKeys "hello"</td><td>Clear any text from the element, and enter text (to the current element)</td></tr>
<tr><td>ClearAndSendKeys &quot;&lt;value&gt;&quot; to id &lt;id&gt;</td><td>ClearAndSendKeys "fred" to id username</td><td>Find an element by id, clear any text from the element, and enter text</td></tr>
<tr><td>SendKey Key.&lt;key&gt;</td><td>SendKey Key.RETURN</td><td>Enters the given key into the current element, without clearing any current content    Note this is to be used for 'special' keys defined by org.openqa.selenium.Keys</td></tr>
<tr><td>SendKeys &quot;&lt;value&gt;&quot;</td><td>SendKeys hello</td><td>Enters text to the current element, without clearing any current content  first</td></tr>
<tr><td>SetCheckBox name=&quot;&lt;name&gt;&quot;, checked=&lt;checked&gt;</td><td>SetCheckBox name="accept", checked=true</td><td>Sets a check box value; deprecated use</td></tr>
<tr><td>SetCheckedBox checked=&lt;checked&gt;</td><td>SetCheckedBox checked=true</td><td>Sets the value of the current element, assumed to be a checkbox to...</td></tr>
<tr><td>SetRadioButton checked=&lt;checked&gt;</td><td>SetRadioButton checked=true</td><td>Sets the value of the current element, assumed to be a radio button to...</td></tr>
<tr><td>SetRadioButton name =&lt;name&gt;, value =&lt;value&gt;, checked =&lt;checked&gt;</td><td>SetRadioButton name=opt_in, value=OFF, checked=true</td><td>Use: FindRadioButton inside tag=&amp;quot;label&amp;quot; with label=&amp;quot;&amp;lt;radio_button_text&amp;gt;&quot;  + SetRadioButton checked=&amp;lt;true&amp;gt; in preference as this will locate the  radio button by visible text rather than the underlying value.    Locates a radio button with a specific value and checks the radio button.</td></tr>
<tr><td>SetRadioButton name=&quot;&lt;name&gt;&quot;, text=&quot;&lt;text&gt;&quot;</td><td>SetRadioButton name="opt_in", text="radio button text"</td><td>Sets the value of a radio button</td></tr>
<tr><td colspan="3"><strong>Location</strong></td></tr>
<tr><td>FindById &lt;id&gt;</td><td>FindById username</td><td>Find an element by it's ID</td></tr>
<tr><td>FindById &lt;id&gt; and text = &quot;&lt;expected&gt;&quot;</td><td>FindById msg_id and text = "Hello World"</td><td>Find the element with id that has the text ....</td></tr>
<tr><td>FindByIdTimeout &lt;id&gt; timeout = &lt;timeout&gt; secs</td><td>FindByIdTimeout username timeout = 15 secs</td><td>Find an element by it's ID with the specified timeout</td></tr>
<tr><td>FindByName &quot;&lt;name&gt;&quot;</td><td>FindByName "named field"</td><td>Find an element using the name attribute of the element</td></tr>
<tr><td>FindByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindByTagAndAttributes tag="input"
          attributes=[type="submit",value="Search"]</td><td>Find an element by tag name and a set of attributes and corresponding  values</td></tr>
<tr><td>FindByTagAndAttributesWithText tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;] with text=&quot;&lt;text&gt;&quot;</td><td>FindByTagAndAttributesWithText tag="input"
          attributes=[type="submit",value="Search"]</td><td>Find an element by tag name and a set of attributes and corresponding  values</td></tr>
<tr><td>FindByXpath &lt;xpath&gt;</td><td>FindByXpath</td><td>Find an id by xpath</td></tr>
<tr><td>FindCheckbox inside tag=&quot;&lt;tag&gt;&quot; with label=&quot;&lt;label&gt;&quot;</td><td>FindCheckbox inside tag="label" with label="a checkbox label"</td><td>Finds a checkbox that is a child of the specified tag, that contains the  specified text; eg.       &amp;lt;pre&amp;gt;      &amp;lt;label&amp;gt;      &amp;lt;input type=&amp;quot;checkbox&amp;quot; name=&amp;quot;checkbox_name&amp;quot; value=&amp;quot;yeah&amp;quot;/&amp;gt;a checkbox &amp;lt;span&amp;gt;label&amp;lt;/span&amp;gt;      &amp;lt;/label&amp;gt;      &amp;lt;/pre&amp;gt;</td></tr>
<tr><td>FindChild ByName name=&quot;&lt;name&gt;&quot;</td><td>FindChild ByName name="child name"</td><td>Finds an element that is a child of the current element using the name  attribute, another Find method should be used first</td></tr>
<tr><td>FindChild ByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindChild ByTagAndAttributes tag="input"
          attributes=[type="submit",value="Search"]</td><td>Finds an element that is a child of the current element using the tag  name and specified attributes, another Find method should be used first</td></tr>
<tr><td>FindChild ByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;] with text=&quot;&lt;text&gt;&quot;</td><td>FindChild ByTagAndAttributes tag="input"
          attributes=[type="submit",value="Search"] with text="bob"</td><td>Finds an element that is a child of the current element using the tag  name, specified attributes and text, another Find method should be used first</td></tr>
<tr><td>FindFirstByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindFirstByTagAndAttributes tag="input"
          attributes=[type="submit",value="Search"]</td><td>Finds the first element by tag name and a set of attributes and  corresponding values</td></tr>
<tr><td>FindFirstChild ByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindFirstChild ByTagAndAttributes tag="input"
          attributes=[type="submit",value="Search"]</td><td>Finds the first child element of the 'current' element using the tag name  and specified attributes, another Find method should be used first</td></tr>
<tr><td>FindFirstChildElementContainingText xpath=&quot;&lt;xpath&gt;&quot; text=&quot;&lt;text&gt;&quot;</td><td>FindFirstChildElementContainingText xpath="li//a" text =
          "Log Out"</td><td>From the current element, apply the xpath selecting the first child that  has the text ...</td></tr>
<tr><td>FindFirstTagElementContainingText tag=&quot;&lt;tag&gt;&quot; text=&quot;&lt;text&gt;&quot;</td><td>FindFirstTagElementContainingText tag="ul"
          text="list item itext"</td><td>Finds an element on the page with the specified tag and containing the specified text</td></tr>
<tr><td>FindFirstTagElementStartingWithText tag=&quot;&lt;tag&gt;&quot; text=&quot;&lt;text&gt;&quot;</td><td>FindTagElementStartingWithText tag="ul" text="list item itext"</td><td>Finds the first html tag that starts with the specified text</td></tr>
<tr><td>FindNthByTagAndAttributes n=&quot;&lt;nth&gt;&quot; tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindNthByTagAndAttributes n=2 tag="input"
          attributes=[type="submit",value="Search"]</td><td>Finds the n th element by tag name and a set of attributes and  corresponding values</td></tr>
<tr><td>FindParentByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;] ThatHasChild tag=&quot;&lt;childTag&gt;&quot; attributes=[&lt;childAttributeString&gt;]</td><td>FindParentByTagAndAttributes tag="table"
          attributes=[class="mytable"] ThatHasChild tag="caption"
          attributes=[class="childClass"]</td><td>Finds an element by tag name and a set of attributes and corresponding  values, that has a child tag element of the specified type that has the  specified attributes..</td></tr>
<tr><td>FindParentByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;] ThatHasChild tag=&quot;&lt;childTag&gt;&quot; text=&quot;&lt;childText&gt;&quot;</td><td>FindParentByTagAndAttributes tag="table"
          attributes=[class="mytable"] ThatHasChild tag="caption"
          text="wahoo"</td><td>Finds an element by tag name and a set of attributes and corresponding  values, that has a child tag element of the specified type and having the  specified text</td></tr>
<tr><td>FindRadioButton inside tag=&quot;&lt;tag&gt;&quot; with label=&quot;&lt;label&gt;&quot;</td><td>FindRadioButton inside tag="label" with label="a radio label"</td><td>Finds a radiobutton that is a child of the specified tag, that contains  the specified text; eg.       &amp;lt;pre&amp;gt;      &amp;lt;label&amp;gt;      &amp;lt;input type=&amp;quot;radio&amp;quot; name=&amp;quot;radio_name&amp;quot; value=&amp;quot;yeah&amp;quot;/&amp;gt;a radio &amp;lt;span&amp;gt;label&amp;lt;/span&amp;gt;      &amp;lt;/label&amp;gt;      &amp;lt;/pre&amp;gt;</td></tr>
<tr><td>FindTagElementWithExactText tag=&quot;&lt;tag&gt;&quot; text=&quot;&lt;text&gt;&quot;</td><td>FindTagElementContainingText tag="ul" text="list item itext"</td><td>Finds an element on the page with the specified tag and text</td></tr>
<tr><td>NavigateTo &lt;url&gt;</td><td>NavigateTo /myApp (will navigate to http://localhost/myApp if
          base.url is set to http://localhost)</td><td>Navigate to a url, if the url begins with http or file, the url will be  used as is, if a relative url is specified then it will be prepended with  the base url property</td></tr>
<tr><td>SwitchFrameToCurrentElement</td><td>SwitchFrameToCurrentElement</td><td>Transfer the focus into the current element (set with a previous Find  method) which should be a frame or iframe</td></tr>
<tr><td>WaitFor &lt;value&gt;</td><td>WaitFor 10</td><td>Wait for the specified number of milliseconds</td></tr>
<tr><td>WaitForPageTitle &quot;&lt;expectedTitle&gt;&quot;</td><td>WaitForPageTitle "My Home Page"</td><td>Wait for the page title to change to the specified value</td></tr>
<tr><td colspan="3"><strong>Miscellaneous</strong></td></tr>
<tr><td>AssertDifferent rememberedValue &quot;&lt;rememberedValueName&gt;&quot; compareToElement &quot;&lt;elementId&gt;&quot;</td><td>AssertDifferent rememberedValue "savedProjectName"
          compareToElement "projectName"</td><td>Compare the text of an element (identified by ID) to a value previously  remembered</td></tr>
<tr><td>AssertEventuallyNotEmpty id=&quot;&lt;elementId&gt;&quot;</td><td>AssertEventuallyNotEmpty mySpan</td><td>Asserts that an element (identified by ID) eventually gets some text  inserted into it (by JavaScript, probably)</td></tr>
<tr><td>AssertPageSourceContains &quot;&lt;expected&gt;&quot;$</td><td>AssertPageSourceContains "foobar"</td><td>Simple text search on page source</td></tr>
<tr><td>AssertSame rememberedValue &quot;&lt;rememberedValueName&gt;&quot; compareToElement &quot;&lt;elementId&gt;&quot;</td><td>AssertSame rememberedValue "savedProjectName" compareToElement
          "projectName"</td><td>Compare the text of an element (identified by ID) to a value previously  remembered - assert they're the same</td></tr>
<tr><td>AssertSelect id=&quot;&lt;id&gt;&quot; text=&quot;&lt;value&gt;&quot; is currently selected</td><td></td><td></td></tr>
<tr><td>AssertSelect id=&quot;&lt;id&gt;&quot; text=&quot;&lt;value&gt;&quot; is not currently selected</td><td></td><td></td></tr>
<tr><td>ClickSubmitButton &quot;&lt;buttonText&gt;&quot;</td><td></td><td></td></tr>
<tr><td>DismissAlert with message &quot;&lt;message&gt;&quot;</td><td></td><td></td></tr>
<tr><td>RememberForScenario textFrom &quot;&lt;elementId&gt;&quot; as &quot;&lt;nameToSaveAs&gt;&quot;</td><td>RememberForScenario textFrom "projectName" as "savedProjectName"</td><td>Grab the text of an element (identified by id) and save it for the  duration of this scenario</td></tr>
<tr><td colspan="3"><strong>Startup / Shutodwn</strong></td></tr>
<tr><td>Shutdown</td><td>Shutdown</td><td>Shuts down the current web driver session</td></tr>
<tr><td>Startup</td><td>Startup</td><td>Starts a new web driver session</td></tr>
<tr><td colspan="3"><strong>Table</strong></td></tr>
<tr><td>AssertTableValue column &lt;column&gt;, row &lt;row&gt; contains text &quot;&lt;text&gt;&quot;</td><td>AssertTableValue column 2, row 3 contains text "Hello Bob"</td><td>Check that a table cell contains the specified text using a 1 based  index. Row 1 is the first  &amp;lt;tr&amp;gt;  beneath a &amp;lt;tbody&amp;gt;</td></tr>
<tr><td>FindElementInRow ByTagAndAttributes tag=&quot;&lt;tag&gt;&quot; attributes=[&lt;attributeString&gt;]</td><td>FindElementInRow ByTagAndAttributes tag="a"
          attributes=[class="link-class",....]</td><td>Find an element within a table row by tag and attributes.</td></tr>
<tr><td>FindElementInRow linkText=&quot;&lt;linkText&gt;&quot;</td><td>FindElementInRow linkText="View"</td><td>Find a link (anchor) element within a table row using the link text as a  discriminator.</td></tr>
<tr><td>FindTableBodyRow row &lt;row&gt;</td><td>FindTableBodyRow row 3</td><td>Locates the table body row, assuming that the table has already been  located Row 1 is the first  &amp;lt;tr&amp;gt;  beneath a &amp;lt;tbody&amp;gt;</td></tr>
<tr><td>FindTableRowWithColumnsThatContainText [&lt;columnText&gt;]</td><td>FindTableRowWithColumnsThatContainText
          ["My Name","Where it all began...","December 19 2012"]</td><td>Find a row in a table where columns exist that contain the specified  text. Not all columns of the table need to specified, however the order  is important. Finding multiple matching results will result in an error.    Once the row has been located, other FindInRow methods can be used that  may in turn refer to and set the 'Current Element', this method does not  set the current element for that reason.</td></tr>
</table>