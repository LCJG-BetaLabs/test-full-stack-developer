# test-full-stack-developer
Repository for full-stack developer written test

Please use NodeJS or Python, with any extra tech stack of your choice.

Kindly create a private repository and invite [lcjg-betalabstech](https://github.com/lcjg-betalabstech) as a collaborator when you feel comfortable to request a review.

Tests are appreciated.

## Expected time to complete
8 - 12 Hours

## Tasks

Hilbert's Grand Hotel is going to launch a campaign online which sells packages including a flight and 1-day accommodation at a very low price.

Here is an example of the packages in JSON:

```js
{
  "packages": [
    { "id": 1, "flight": "Flight-1", "stay": "2022-08-09", "price": 100, quota: 1 },
    { "id": 2, "flight": "Flight-2", "stay": "2022-08-09", "price": 100, quota: 2 },
    { "id": 3, "flight": "Flight-3", "stay": "2022-08-10", "price": 100, quota: 2 },
    { "id": 4, "flight": "Flight-3", "stay": "2022-08-11", "price": 100, quota: 2 }
  ]
}
```

### Frontend

Please implement the following features in frontend

- a page to place select pacakges and place an order with an email
- a result page that shows the order with details, or simply a fail message
- a page to show an order by order ID with the email used when purchase the order

### Backend

Please implement the following features in backend


- an endpoint to reserve flight
  - Please fail 50% of the reservation randomly
- an endpoint to reserve a hotel room
  - a valid flight ticket number MUST be provided in order to make the reservation
- an endpoint to purchase a package
  - only allow to purchase package with quota > 0, if quota runs out, throw an exception
  - consume 1 quota before reserving flight and hotel room as to avoid oversale
  - release the quota (add back 1) once either flight or hotel room reservation fail
- an endpoint to retrieve the order by ID and email



### Design and explanations

Please briefly explain why/how did you choose the tech stack, e.g. Docker, ReactJS/Vue.js, ant-design/Material UI/CoreUI, database, web framework, ORM/ODM, etc

