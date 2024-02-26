## Deploy JSON Server to Vercel

A template to deploy [JSON Server](https://github.com/typicode/json-server) to [Vercel](https://vercel.com), allow you to run fake REST API online!

Demo from this repository: 

1. [https://json-server-in.vercel.app](https://json-server-vercel-kappa-bice.vercel.app/)
2. [https://json-server-in.vercel.app/api/posts](https://json-server-vercel-kappa-bice.vercel.app/api/products)

![Powered by Vercel](https://images.ctfassets.net/e5382hct74si/78Olo8EZRdUlcDUFQvnzG7/fa4cdb6dc04c40fceac194134788a0e2/1618983297-powered-by-vercel.svg)

### How to use

1. Click "**Use this template**" or clone this repository.
2. Update or use the default [`db.json`](./db.json) in the repository.
3. Sign Up or login into [Vercel](https://vercel.com).
4. From the Vercel dashboard, click "**+ New Project**" then "**Import**" your repository.
5. In the "**Configure Project**" screen, leave everything default and click "**Deploy**".
6. Wait until deployment is done, and your own JSON server is ready to serve!

## Default `db.json`

```json
{
  "products": [
    {
      "id": 1,
      "title": "Viúva Negra",
      "price": 9.99,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/viuva-negra.png"
    },
    {
      "id": 2,
      "title": "Shang-chi",
      "price": 30.99,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/shang-chi.png"
    },
    {
      "id": 3,
      "title": "Homem Aranha",
      "price": 29.9,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/spider-man.png"
    },
    {
      "id": 5,
      "title": "Morbius",
      "price": 1.5,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/morbius-1.png"
    },
    {
      "id": 6,
      "title": "Batman",
      "price": 21.9,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/the-batman.png"
    },
    {
      "id": 4,
      "title": "Eternos",
      "price": 17.9,
      "image": "https://wefit-react-web-test.s3.amazonaws.com/eternals.png"
    }
  ]
}
```

## Enable write operations

By default, only GET operation is allowed, thanks to the contribution by [@VicAv99](https://www.github.com/VicAv99) at [#6](https://github.com/kitloong/json-server-vercel/issues/6), we can now enable write operations as well.

You can find the example code in [`api/server.js`](./api/server.js).

## Reference

1. https://github.com/typicode/json-server
2. https://vercel.com
3. https://shadowsmith.com/how-to-deploy-an-express-api-to-vercel
