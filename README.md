# beckn-one-registry

## Setup Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/beckn/beckn-one-registry
   cd beckn-one-registry
   ```

2. **Install dependencies**

   ```bash
   npm install -f
   ```

3. **Start MySQL database**

   ```bash
   docker-compose up -d
   ```

4. **Create environment file**

   ```bash
   cp .env.example .env
   ```

5. **Build registry plugins**

   ```bash
   cd src/plugins/plugins/registry
   npm install -f
   npm run build
   ```

6. **Return to root directory**

   ```bash
   cd ../../../../
   ```

7. **Start the application**

   ```bash
   npm run dev
   ```

8. **Login to Strapi server**
   - If prompted to login, use the following credentials shared over email
   - If no login prompt appears, you can create a new user account
