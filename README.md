# react-native-multiple-select-list
Multiple select list with search bar

Install :
```
npm install --save react-native-multiple-select-list
```
Example usage :
```javascript
import CustomMultiPicker from "react-native-multiple-select-list";

<CustomMultiPicker
  options={processedField.options}
  search={true} // should show search bar?
  multiple={true} //
  placeholder={I18n.t("discussions_search_user_placeholder")}
  placeholderTextColor={'#757575'}
  returnValue={"label"} // label or value
  callback={(res)=>{ console.log(res) }} // callback, when selections changed.
  rowBackgroundColor={"#eee"}
  rowHeight={40}
  rowRadius={5}
  iconColor={"#00a2dd"}
  iconSize={30}
  selectedIconName="ios-checkmark-circle-outline"
  unselectedIconName="ios-radio-button-off-outline"
  scrollViewHeight={130}
/>
```

![react-native-multiple-select-list](https://raw.githubusercontent.com/ataomega/react-native-multiple-select-list/master/screenshot.png)


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
rowBackgroundColor: background color for each row in list
rowHeight: row height
rowRadius: row border radius
iconColor: icon color for checked/unchecked icons and search icon also border color of search bar
iconSize: icon size for checked/unchecked icons
selectedIconName: selected/checked icon name (react-native-vector-icons/Ionicon)
unselectedIconName: unselected/unchecked icon name (react-native-vector-icons/Ionicon)
scrollViewHeight: scrollview height (list of items)

By Ata.
ataomega@gmail.com
