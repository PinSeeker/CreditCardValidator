Inspired from [https://github.com/MaxKramer/ObjectiveLuhn]()


# Installation
`pod "CreditCardValidator"`

# Usage
## Validating

```Swift
let number = "1234 5678 9123 4567"
   
if CreditCardValidator(number).isValid {
  // Card number is valid
} else {
  // Card number is invalid
}

```

## Detect Card Type

```Swift
let number = "1234 5678 9123 4567"
   
if let type = CreditCardValidator(number).type {
	print(type.name) // Visa, Mastercard, Amex etc.
} else {
	// I Can't detect type of credit card
}

```
## Check type and validation

```Swift
let number = "1234 5678 9123 4567"
   
if CreditCardValidator(number).isValid(for: .visa) {
	// Card number is valid and type is .visa
} else {
	// I Can't detect type of credit card
}

```

## Supported types
* Amex
* Visa
* MasterCard
* Maestro
* DinersClub
* JCB
* Discover
* UnionPay
* Mir

# Contribution
Contributions are very welcomed 👍😃.