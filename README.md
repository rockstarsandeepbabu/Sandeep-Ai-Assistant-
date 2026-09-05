# Sandeep AI Assistant — ढा़ढ़वा पंचायत का डिजिटल जन-सहायक

यह Cloudflare Workers + Workers AI पर आधारित starter project है। इसमें OpenAI API key की जरूरत नहीं है।

## Deploy
1. Cloudflare account में लॉगिन करें।
2. Workers & Pages → Create application → Workers → Create Worker.
3. इस project को GitHub से जोड़ सकते हैं या Wrangler से deploy कर सकते हैं।
4. `wrangler.toml` में account/project settings जरूरत के अनुसार रखें।
5. Workers AI binding (`AI`) सक्षम करें।
6. `npm install` और `npx wrangler deploy` चलाएँ।

## Local development
```bash
npm install
npx wrangler dev
```

## जानकारी अपडेट करना
`src/knowledge.js` में KNOWLEDGE_BASE बदलें। बाद में नई जानकारी जोड़ना आसान रहेगा।

## सुरक्षा
AI binding server-side है। कोई API key browser में नहीं रखी गई है।
