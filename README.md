# Connecting a Custom Domain to Vercel via Upperlink.ng

## Step 1: Register Your Domain on Upperlink

1. Sign in to your **Upperlink dashboard** at [upperlink.ng](https://upperlink.ng)
2. Navigate to the **Domains** section and register your desired domain
3. During registration, when prompted to select a DNS management option, **ensure you tick/enable DNS management**
4. Remove the default nameservers and replace them with Vercel's nameservers:
   - `ns1.vercel-dns.com`
   - `ns2.vercel-dns.com`
5. Save your changes and complete the registration process
6. Proceed with payment — **Paystack is the recommended payment method**

---

## Step 2: Deploy Your Project on Vercel

1. Log in to your **Vercel account** at [vercel.com](https://vercel.com)
2. Click **Add Project** and select the GitHub repository you want to deploy
3. Follow the prompts to configure and deploy your project
4. Wait for the deployment to complete successfully

---

## Step 3: Add Your Custom Domain on Vercel

1. Once deployed, open your project on Vercel
2. Go to the **Domains** tab and click **Add Existing Domain**
3. Enter the domain you registered on Upperlink and confirm

> At this point, Vercel may display an **"Invalid Configuration"** error regarding DNS records — this is expected. Do not be alarmed.

---

## Step 4: Verify and Connect the Domain

1. On the error screen, locate and click the **"Vercel DNS"** tab
2. You will see a prompt: *"Update your domain's nameservers to enable Vercel DNS"* — confirming the nameservers you already set in Step 1:
   - `ns1.vercel-dns.com`
   - `ns2.vercel-dns.com`
3. Click the **Refresh** button
4. Wait approximately **2 minutes** for DNS propagation
5. Click **Refresh** again

Your domain should now show as successfully connected to your Vercel project. 🎉

---

> **💡 Tip:** DNS propagation can sometimes take a few minutes. If the domain doesn't connect immediately after the first refresh, wait a moment longer and try again.
