# react-native-multiple-select-list
Multiple select list with search bar

### Install :
```sh
npm install --save react-native-multiple-select-list
```
### Example usage :
```javascript
import CustomMultiPicker from "react-native-multiple-select-list";

const userList = {
  "123":"Tom",
  "124":"Michael",
  "125":"Christin"
}

//const userList = {
//  "123":<View><Text>Tom</Text></View>,
//  "124":<View><Text>Michael</Text></View>,
//  "125":<View><Text>Christin</Text></View>
//}

<CustomMultiPicker
  options={userList}
  search={true} // should show search bar?
  multiple={true} //
  placeholder={"Search"}
  placeholderTextColor={'#757575'}
  returnValue={"label"} // label or value
  callback={(res)=>{ console.log(res) }} // callback, array of selected items
  rowBackgroundColor={"#eee"}
  rowHeight={40}
  rowRadius={5}
  searchIconName="ios-checkmark"
  searchIconColor="red"
  searchIconSize={30}
  iconColor={"#00a2dd"}
  iconSize={30}
  selectedIconName={"ios-checkmark-circle-outline"}
  unselectedIconName={"ios-radio-button-off-outline"}
  scrollViewHeight={130}
  selected={["Tom", "Christin"]} // list of options which are selected by default
/>
```

![react-native-multiple-select-list](https://raw.githubusercontent.com/ataomega/react-native-multiple-select-list/master/screenshot.png)


### Props:
| Prop | Type | Description |
| ------ | ------ | ------ |
| options | Object | list of options/items |
| search | Boolean | if the search bar should be shown or not |
| multiple | Boolean | if user can select multiple options or not. if you select an item which is already selected, it will be unselected. if multiple is disabled, it will work like radio buttons. |
| placeholder | String | placeholder text for search bar |
| placeholderTextColor | String | placeholder text color for search bar |
| returnValue | String | should it return keys of selected options or values? |
| callback | Function | whenever user selects or changes selections it will be called. |
| rowBackgroundColor | String | background color for each row in list |
| rowHeight | Integer | row height |
| rowRadius | Integer | row border radius |
| searchIconName | String | Name of the vector icon displayed on the search bar |
| searchIconSize | Integer | icon size for the icon displayed on the search bar |
| searchIconColor | String | icon color the icon displayed on the search bar |
| iconSize | Integer | icon size for checked/unchecked icons |
| iconColor | String | icon color for checked/unchecked icons and search icon also border color of search bar |
| iconSize | Integer | icon size for checked/unchecked icons |
| selectedIconName | String | selected/checked icon name (react-native-vector-icons/Ionicon) |
| unselectedIconName | String | unselected/unchecked icon name (react-native-vector-icons/Ionicon) |
| scrollViewHeight | Integer |scrollview height (list of items) |
| selected | Object | list of options which are selected by default |
| scrollViewStyle | Object | Style object for scrollView that holds all items
| itemStyle | Object | Style object for the touchableOpacity of each item
| labelStyle | Object | Style object for the text label
| selectedIconStyle | Object | style object for the icon when selected
| unselectedIconStyle | Object | style object for the icon when unselected

### Author:
Ata Mohammadi.
atasmohammadi@gmail.com
