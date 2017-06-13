# react-native-multiple-select-list
Multiple select list with search bar

![react-native-multiple-select-list](https://raw.githubusercontent.com/ataomega/react-native-multiple-select-list/master/screenshot.png)

Example usage :
```
<CustomMultiPicker
  options={processedField.options}
  search={true} // should show search bar?
  multiple={true} //
  placeholder={I18n.t("discussions_search_user_placeholder")}
  placeholderTextColor={'#757575'}
  returnValue={"label"} // label or value
  callback={(res)=>{ console.log(res) }} // callback, when selections changed.
/>
```

By Ata.
ataomega@gmail.com
