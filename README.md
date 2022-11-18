# Bookshop Demo

Bookshop is a virtual online bookstore application through which you can find books of various categories and rate the books.

You can perform CRUD operations such as viewing book details, adding and deleting ratings, editing book inventory, etc.

## 🔥 Visit Live Demo

[👉 Click here to visit demo](https://tidb-prisma-vercel-demo.vercel.app/)

> Powered by TiDB Cloud, Prisma and Vercel.

![image](https://user-images.githubusercontent.com/56986964/183592978-42d702eb-b5fc-4285-b081-30a50803fe1a.png)

## Deploy on Vercel

### 🧑‍🍳 Before We Start

Create a [TiDB Cloud](https://tidbcloud.com/) account and get your free trial cluster.

### 🚀 One Click Deploy

You can click the button to quickly deploy this demo if already has an TiDB Cloud cluster.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?demo-title=TiDB%20Cloud%20Starter&demo-description=A%20bookstore%20demo%20built%20on%20TiDB%20Cloud%20and%20Next.js.&demo-url=https%3A%2F%2Ftidb-prisma-vercel-demo.vercel.app%2F&demo-image=%2F%2Fimages.ctfassets.net%2Fe5382hct74si%2F2HMASOQn8hQit2IFi2hK3j%2Fcfe7cc2aeba4b8f6760a3ea14c32f707%2Fscreenshot-20220902-160324_-_Chen_Zhen.png&project-name=TiDB%20Cloud%20Starter&repository-name=tidb-cloud-starter&repository-url=https%3A%2F%2Fgithub.com%2Fpingcap%2Ftidb-prisma-vercel-demo&from=templates&integration-ids=oac_coKBVWCXNjJnCEth1zzKoF1j)

> Integration will guide you connect your TiDB Cloud cluster to Vercel.

<details>
  <summary><h3>Manually Deploy (Not recommended)</h3></summary>

#### 1. Get connection details

You can get the connection details by clicking the `Connect` button.

![image](https://user-images.githubusercontent.com/56986964/183590385-0e688bac-8c4b-4988-ad02-692650b4c5a8.png)

Get `User` and `Host` field from the dialog.

> Note: For importing initial data from local, you can set an Allow All traffic filter here by entering an IP address of `0.0.0.0/0`.

![image](https://user-images.githubusercontent.com/56986964/183590950-93fb5778-128b-40e1-ab85-33994bd6f4de.png)

Your `DATABASE_URL` should look like `mysql://<User>:<Password>@<Host>:4000/bookshop`

#### 2. Deploy on Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fpingcap%2Ftidb-prisma-vercel-demo&repository-name=tidb-prisma-vercel-demo&env=DATABASE_URL&envDescription=TiDB%20Cloud%20connection%20string&envLink=https%3A%2F%2Fdocs.pingcap.com%2Ftidb%2Fdev%2Fdev-guide-build-cluster-in-cloud&project-name=tidb-prisma-vercel-demo)

![image](https://user-images.githubusercontent.com/56986964/199161016-2d236629-bb6a-4e3c-a700-c0876523ca6a.png)

</details>

## Deploy on Netlify

### 🧑‍🍳 Before We Start

1. Create a [TiDB Cloud](https://tidbcloud.com/) account and get your free trial cluster.
2. Create a [Netlify](https://app.netlify.com/signup) account.

### 1. Get connection details

1. Navigate to your TiDB Serverless cluster's dashboard.
2. Get **Endpoint**, **Port** and **User** field from the Connection tab.
3. Build your **DATABASE_URL**: `mysql://<User>:<Password>@<Endpoint>:<Port>/bookshop`

![image](https://user-images.githubusercontent.com/35677990/202609001-ecf07f3d-a7a3-4376-9b7d-54f4096aaec6.jpg)

You will use this DATABASE_URL string to connect to TiDB Serverless cluster later.

### 2. Deploy on Netlify

The **Deploy to Netlify** button will take you Netlify's deployment page. Then Netlify will help to clone this job to your own GitHub repository and automatically deploy it.

[![Deploy to Netlify button](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Daemonxiao/tidb-prisma-vercel-demo)

1. Click the **Deploy to Netlify** button.
2. Click **Connect to GitHub** and authenticate GitHub account.
3. Fill in **Repository name** for your own GitHub repository.
4. Click **Save & Deploy**.
   ![image](https://user-images.githubusercontent.com/35677990/202630299-ba4802b6-8535-486d-b767-c6ef0acc01a8.jpg)
5. Navigate to **Site setting** panel.
6. Click **Add a variable** in the **Environment variables** sidebar.
   ![image](https://user-images.githubusercontent.com/35677990/202631704-6e463edf-7a2e-4cce-a9c7-98853167424f.jpg)
7. Enter "DATABASE_URL" in the **Key** field.
8. Enter the DATABASE_URL string, set in the previous step, in the **Values** field.
9. Click **Create variable** to complete adding environment variable.
   ![image](https://user-images.githubusercontent.com/35677990/202632393-8a2e5f56-5b04-4585-931b-34a836e7df37.jpg)
10. 

## 📖 Development Reference

### Prisma

[Prisma Deployment Guide](https://www.prisma.io/docs/guides/deployment/deploying-to-vercel)

### Bookshop Schema

[Bookshop Schema Design](https://docs.pingcap.com/tidbcloud/dev-guide-bookshop-schema-design)
