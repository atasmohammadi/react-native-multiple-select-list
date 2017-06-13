# react-native-multiple-select-list
Multiple select list with search bar

![react-native-multiple-select-list](https://raw.githubusercontent.com/ataomega/react-native-multiple-select-list/master/screenshot.png)

Example usage :
```javascript
<CustomMultiPicker
  options={processedField.options}
  search={true} // should show search bar?
  multiple={true}
  placeholder={I18n.t("discussions_search_user_placeholder")}
  placeholderTextColor={'#757575'} // color
  returnValue={"label"} // label or value
  callback={(res)=>{ console.log(res) }} // callback, when selection changes.
/>
```
Props:
options: an object like
```javascript
{
  key: value
}
```
search: if search bar should be shown or not
multipe: if user can select multiple options or not. if you select an item which is already selected, it will be unselected. if multiple is disabled, it will work like radio buttons.
placeholder: placeholder text for search bar
placeholderTextColor: placeholder text color for search bar
returnValue: should it return keys of selected options or values?
callback: whenever user selects or changes selections it will be called.

NPM package will be released soon.

By Ata.
ataomega@gmail.com
