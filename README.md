# Custom Commands for Streamlabs Chatbot
### List of custom commands that maybe you won't find in the documentation.

## Requirements

* [Streamlabs Chatbot](https://streamlabs.com/chatbot)

## Commands

### !give
>$addpoints("$target","$num2","$num2","Give $value $currencyname to $target.","Fail to give $currencyname.")

Usage
>!give user value

Example
>!give batera 10

### !remove
>$removepoints("$target","$num2","$num2","Removed $value $currencyname from $target.","Fail to remove $currencyname.","false")

Usage
>!remove user value

Example
>!remove batera 10

### !transfer
>$givepoints("$user","$target","$num2","$user transferred $value $currencyname to $target.","$user: You don't have enough $currencyname!","false")

### !transfer (Discounting 10%)
>$addpoints("$target","$math[$num2-($num2*0.1)]","$math[$num2-($num2*0.1)]","$user transferred $value $currencyname to $target.","Fail to transfer $currencyname.")
>$removepoints("$user","$num2","$num2","","Error.","false")

Usage
>!transfer user value

Example
>!transfer batera 10

### Give points for all viewers in the chat

Usage
>!currency add +viewers value

Example
>!baquetas add +viewers 25
