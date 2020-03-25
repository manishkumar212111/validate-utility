# validate-utility

This package is used to validate user input and check many types of regexs.

# Installation

Run : `npm i validate-utility`

## Usage

| Function name | Description                    |
| ------------- | ------------------------------ |
| `validate(e.target , id , callBack)`      | `This method is used with input attribute as used in sample code`       |
| `url(value)`      | `Validate URL.`       |
| `email(value)`      | `Validate email.`       |
| `alnum(value)`      | `Validate string with alpha and numeric only.`       |
| `alnumwithspace(value)`      | `Validate alpha and numeric string with space .`       |
| `alpha(value)`      | `Validate string contains alphabets .`       |
| `number(value)`      | `Validate string if it only contains number.`       |
| `postcode(value)`      | `Validate postcode or zipcode.`       |
| `mobile(value)`      | `Validate mobile number.`       |
| `pancard(value)`      | `Validate pancard number.`       |
| `DateBelow2000(value)`      | `Validate date before 2000.`       |
| `DateBelow2000R(value)`      | `Validate date after 2000.`       |
| `fullnamewithspace(value)`      | `Validate full name with space.`       |
| `voterID(value)`      | `Validate voter id.`       |
| `dl(value)`      | `Validate driving licence.`       |
| `passport(value)`      | `Validate passport.`       |
| `timeString(value)`      | `Validate if string is timestring.`       |
| `dateString(value)`      | `Validate datestring.`       |
| `hexadecimal(value)`      | `Validate string is hesadecimal or not.`       |
| `hexColor(value)`      | `Validate staring has hexcolor.`       |
| `ipv4(value)`      | `Validate IP in v4 format.`       |
| `ipv6(value)`      | `Validate IP in v6 format.`       |
| `ipV4V6(value)`      | `Validate IP in v4 and v6 both.`       |
| `ip(value)`      | `Validate only IP.`       |
| `vehiclenumber(value)`      | `Validate vehicle number.`       |
| `pan(value)`      | `Validate pan.`       |
| `minLength(value , minLength)`      | `This method is used to validate minLength.`       |
| `maxLength(value , maxLength)`   | `This method is used to validate maxLength.`     |
| `required(value)`   | `This method checks if field is required.`     |
| `isEmpty(value)`   | `This method checks if string is empty.`     |
| `minValue(value , minValue)`   | `This method checks minimum value for numbers.`     |
| `equalTo(value1 , value2)`   | `This method checks equality.`     |
| `equalTo(value1 , value2)`   | `This method checks equality.`     |
| `isChecked(selector)`   | `This methods checks if checkbox is checked.`     |

Note : It return true if validation is successfull



## Sample Code

```\
    function cb (error , id , selector) {
       console.log(error);
       it prints {
              status: true,
              message: ""}
       }
    <input type="text"   
       data-vu-err-msg="this is error message"
       onKeyUp={(e) => validateUtility.validate(e.target , "tets" , cb }) } 
       onKeyPress={(e) => validateUtility.stopDefault(e)}
       data-vu-type="required,minLength,alpha" // type of validation required (any methid name can be used here like mobile,url,email etc
       data-vu-min-length="6"
       data-vu-err-msg="This is error message"
       //data-vu-min-value="8"
    /> 
```
