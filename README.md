# FlatLoan

Angular 6 is the latest version(as of today Jun 5th, 2018) of Angular framework.

Ngrx is a collection of packages that makes it easy to manage state of Angular applications.

You can visit [Angular site]() and [Ngrx site]() for more information.

## Description

The focus of this walkthrough will be "the use of ngrx to store and distribute data among angular components".

We will be using "Flat Loan" as an example application.

Flat Loan is a zero interest lending platform, where User A(lender or person with money), gives money(Amount) to User B(borrower or person with no money). Then in the future User B will give back some amount to User A in multiple installments until all Amount is given back.

## End Goal

By end of this walkthrough, you should be able to
* TODO
* TODO
* TODO
@TODO add a link to working app.

## Step by Step

* Domain model
We need to store the `loan`, which is basically an aggreement that the `lender` has given some `amount` of money to the `borrower` for some `reasons`.
```typescript
interface ILoan {
  lender: IUser;
  borrower: IUser;
  amount: number;
  reason: string;
}
```

We also need to store the `payback`, which will indicate to the `lender` that the `borrower` has paid some `amount` for a given `loan`.
```typescript
interface IPayback {
  amount: Number;
  loan: ILoan;
}
```

```typescript
interface IUser {
  name: string;
  identification: string;
  contact: string;
  photo: ILoan;
}
```

* 

## Result
