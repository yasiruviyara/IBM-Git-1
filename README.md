# SSH Key Creation

```
ssh-keygen -t rsa -b 4096 -C "<your email address>" [ optinal check  >> cd ~/.ssh && ls after come main derc]

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

```
# Add SSH to Repo 

```
cat ~/.ssh/id_rsa.pub (or clip)
```

```
clip < C:\Users\User/.ssh/id_rsa.pub.
```
(SSH and GPG keys )

# env protect
```
.env
.env.*
```
vite prot config

```
import { defineConfig, loadEnv } from 'vite'
import react from '@vitejs/plugin-react-swc'

// https://vitejs.dev/config/
export default defineConfig(({ mode, }) => {

  // eslint-disable-next-line no-undef
  const env = loadEnv(mode, process.cwd(), '')
  
  const port = env.VITE_FRONTEND_PORT || 3000

  return {
    plugins: [react()],
    server: {
      host: true,                 
      port: parseInt(port),        
      
    },
    
  }
})
```
