# E-commerce Application with Payment Gateway Integration
[![ci](https://github.com/ttiimmothy/e-commerce-application-with-payment-gateway-integration/actions/workflows/ci.yml/badge.svg)](https://github.com/ttiimmothy/e-commerce-application-with-payment-gateway-integration/actions/workflows/ci.yml)

An e-commerce application is built with multiple payment gateway integrations and customized plugins addons. It uses **Typescript**, **React** amd **Next.js**. It uses **Tailwind CSS** and **RadixUI** for CSS usage. It uses **redux** to do the state management. For fetching and payment, **axios** and **strapi** are implemented. **MongoDB** is used for data storage.

## 🎯 Features

- [ ] Product Lists UI
- [ ] Checkout Page
- [ ] Add new payment gateway and plugins

### Adding a New Payment Method

To add a new payment method, follow these steps:

1. **Create Payment Method Class:**
   - Create a new class for the payment method, extending the `PaymentMethod` base class.

2. **Implement Payment Logic:**
   - Implement the necessary methods such as `authenticate`, `validate`, `charge`, etc., according to the requirements of the new payment method.

3. **Configure Payment Method:**
   - Add configuration settings for the new payment method in the `paymentMethods.json` file.

4. **Instantiate Payment Method:**
   - Use the `PaymentMethodFactory` to instantiate the new payment method with the appropriate configuration.

5. **Integrate with UI:**
   - Update the UI to include an option for the new payment method and handle its selection.

For detailed examples and best practices, refer to the existing payment method implementations (e.g., `CreditCardPayment`, `PayPalPayment`).

## 🔧 Next.js Instruction

### Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

### Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

### Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## License

E-commerce Application with Payment Gateway Integration is licensed under [Apache-2.0 License](LICENSE).
