## Code coverage example

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer)
{
  return customer.age >= 18;
}
```

```csharp
// Test
var customer = new Customer { name: 'Professor X', age: 96 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

<!-- .element class="flavor-csharp" -->

```javascript
// Production code
function isAllowedToBuyAlcohol(customer) 
{
  return customer.age >= 18;
}
```

```javascript
// Test
var customer = { name: 'Professor X', age: 96 };
expect(isAllowedToBuyAlcohol(customer)).to.equal(true);
```

<!-- .element class="flavor-javascript" -->

What is the code coverage here?

😞 100% 😞 <!-- .element class="fragment" data-fragment-index="0" -->