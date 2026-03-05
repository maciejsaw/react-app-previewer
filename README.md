# React App Previewer

A lightweight, shareable React component previewer. Paste React code and instantly preview it—no build process required. Perfect for sharing quick prototypes, design mockups, and component examples with teammates and clients.

## 🎯 Use Cases

### **1. Quick Prototyping**
- Design and test UI components on the fly
- Experiment with React hooks and component logic
- Iterate rapidly without setting up a dev environment

### **2. AI-Generated Code Preview**
- Paste React code from **ChatGPT**, **Claude**, **Gemini**, or any AI assistant
- Instantly see what the generated component looks like
- Verify functionality before copying to your project

### **3. Collaboration & Sharing**
- Share component previews with non-technical stakeholders
- Get feedback on designs without complex setup
- No installation, no build steps—just a link

### **4. Learning & Teaching**
- Share React code snippets with learners
- Create interactive documentation
- Demo components in presentations or tutorials

### **5. Code Review & Feedback**
- Share component implementations as shareable links
- Team members can view and test live without cloning
- Perfect for remote code reviews

## ✨ Features

- ✅ **Instant Preview**: Run React code instantly in your browser
- ✅ **Shareable Links**: Encode your component in the URL for easy sharing
- ✅ **No Setup Required**: Works entirely in the browser
- ✅ **Tailwind CSS**: Full Tailwind CSS support pre-configured
- ✅ **Lucide Icons**: 400+ Lucide React icons available
- ✅ **Live Error Display**: See errors in real-time
- ✅ **Dark Mode Support**: Built-in dark mode via Tailwind

## 🚀 How to Use

### **Step 1: Get Your React Code**

Paste a React component from an AI assistant or write your own. Your code should export a default component named `App`:

```jsx
import React, { useState } from 'react';

export default function App() {
  const [count, setCount] = useState(0);

  return (
    <div className="flex items-center justify-center min-h-screen bg-gradient-to-br from-blue-500 to-purple-600">
      <div className="bg-white p-8 rounded-lg shadow-xl text-center">
        <h1 className="text-3xl font-bold text-gray-800 mb-4">Counter App</h1>
        <p className="text-6xl font-bold text-blue-600 mb-6">{count}</p>
        <button
          onClick={() => setCount(count + 1)}
          className="bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-6 rounded-lg transition"
        >
          Increment
        </button>
      </div>
    </div>
  );
}
```

### **Step 2: Paste into the Editor**

1. Visit the [React App Previewer](https://react-app-previewer.vercel.app) (or your deployed instance)
2. Click in the text area
3. Paste your React component code

### **Step 3: Click "Run & Preview Fullscreen"**

The component will render instantly. You'll see:
- The live preview in fullscreen
- Any errors displayed at the top
- The code encoded in the URL

### **Step 4: Share the URL**

The URL in your browser now contains the encoded React code. Copy and share it with:
- **Team members** - they see the preview immediately
- **Clients** - no setup needed on their end
- **Social media** - share interactive design prototypes
- **Chat/Email** - send the link directly

**Example shareable URL:**
```
https://react-app-previewer.vercel.app/#eJydUckOwjAM/RXLGJSW6nHgwAFxoBd4rp2UpJr...
```

### **Step 5: Editing & Refreshing**

- **To go back to editing**: Click the browser back button
- **To update code**: Modify the code in the editor and click "Run & Preview Fullscreen" again
- **To save**: The URL is your "save"—bookmark or share it

## 💡 Example Workflows

### **Using ChatGPT/Gemini to Claude:**

1. Ask your AI assistant: *"Create a React component for a beautiful login form with Tailwind CSS"*
2. Copy the generated code
3. Paste into React App Previewer
4. Click "Run & Preview"
5. Share the URL with your team

### **Design Review Process:**

1. Designer uses AI to generate a component mockup
2. Previews it in React App Previewer
3. Shares the link in Slack/Teams
4. Stakeholders click the link and see the live preview
5. Feedback collected, code refined, new URL generated

### **Teaching React:**

1. Create example components
2. Generate shareable URLs
3. Include URLs in lesson materials
4. Students can experiment and modify in their browser
5. No environment setup required

## 🛠️ Technical Details

### **Supported Libraries**

- **React 18.2.0** - Core React library
- **Tailwind CSS 3** - Utility-first CSS framework
- **Lucide React** - Icon library with 400+ icons

### **Import Examples**

```jsx
import React, { useState, useEffect } from 'react';
import { Heart, Star, Settings } from 'lucide-react';

export default function App() {
  return (
    <div className="flex gap-2">
      <Heart className="w-6 h-6 text-red-500" />
      <Star className="w-6 h-6 text-yellow-500" />
      <Settings className="w-6 h-6 text-gray-500" />
    </div>
  );
}
```

### **URL Encoding**

- Code is encoded to Base64 URL-safe format
- Max URL length: ~2000 characters (browser limit)
- Keep components reasonably sized for sharing

### **Browser Requirements**

- Modern browser with ES2015+ support
- No extensions or package installations needed
- Works offline (after initial load)

## ⚠️ Limitations

- **No npm packages**: Only React, Tailwind, and Lucide available
- **No server-side code**: Client-side execution only
- **URL length**: Very large components may exceed URL limits
- **No persistent storage**: Refresh the page and you're back to the editor
- **Same-origin policy**: External APIs must allow CORS

## 🎨 Tips & Best Practices

1. **Keep it modular** - Break complex UIs into smaller components
2. **Use Tailwind classes** - Style everything with Tailwind utilities
3. **Test in different browsers** - Ensure compatibility
4. **Share immediately** - The URL is your version control
5. **Avoid external APIs** - Unless they support CORS
6. **Use placeholder data** - Mock data is better than real API calls

## 🚀 Deployment

Deploy your own instance:

1. **Vercel** (Recommended):
   ```bash
   vercel
   ```

2. **GitHub Pages**: Deploy `index.html` directly
3. **Netlify**: Connect your repository and deploy

## 📝 License

MIT - Feel free to fork and modify

## 🤝 Contributing

Found a bug or have a feature request? Open an issue or submit a pull request!

---

**Happy coding! 🎉**
