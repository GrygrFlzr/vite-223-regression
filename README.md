## Steps

```bash
npm i
npm run dev
```

Start with http://localhost:3000/no-router/a

1. Click button, assert clicks = 1
2. Go to b, assert clicks = 0
3. Click button, assert clicks = 1
4. Go to a, assert clicks = 1
   (success on Vite 2.2.2, fails on Vite 2.2.3)
5. Go to b, assert clicks = 0

Update Vite from 2.2.2 to 2.2.3 and repeat
