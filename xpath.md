#xpath
select element with a given class
> `//*[contains(@class, 'test')`

select element with text
>`//li[text()='January'`]

>*or

>`//li[.='January']`

two levels (smells?)
>`//li[contains(@class, 'project-user')]/label[text()='Rie Tanaka']"`

xpath selector for an element whose container should be visible
>`//div[not(contains(@style,'display:none'))]/button[.='something']`

selector for multiple attributes
>`//div[contains(@class,'pretty') and not(contains(@style, 'display:none'))]`
>`//div[text()='test' and contains(@class, 'pretty')]`

selector for any element that contains given text
>`//*[contains(text(),'giventext']`

