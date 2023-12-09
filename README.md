# Vite + React + Typescript Boilerplate

1. node type 설치

```
pnpm add -D @types/node
```

2. vercel 배포 시 라우팅 설정 필요
   => vercel.json 복사 및 붙여넣기

3. 절대경로 설정
   => vite.confing.ts 와 tsconfig.json 설정
   => 복사 밑 붙여넣기

4. svg 컴포넌트 사용 시 svgr 설치 / vite-env.d.ts에 svgr관련 코드 추가

```
pnpm add -D vite-plugin-svgr
```

```
/// <reference types="vite-plugin-svgr/client" />
```

5. eslint, prettier 설정
   => .eslintrc.cjs, .prettierrc, .prettierignore 복사 및 붙여넣기

---

### Tailwind CSS 설정

1. 설치 및 초기화

```
pnpm add -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

2. tailwind.config.js 설정

=> tailwind.config.js 복사 및 붙여넣기

3. index.css (globals.css) 설정

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

### Css-in-js 설정 (styled-components or emotion)

1. 설치

- emotion

```
pnpm add @emotion/react @emotion/styled
```

- styled-components

```
pnpm add styled-components
```

2. reset, font, global 스타일 적용
   => reset.css, fonts.css, globals.css 복사 및 붙여넣기

3. 반응형일 경우 media.ts의 break-point 설정 및 ThemeProvider에 적용

```
<ThemeProvider theme={{ media }}>
   ...
</ThemeProvider>
```
