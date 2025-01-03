# ClickEffects - Next.js Particle Effects Project

## Overview
This project is a Next.js application that demonstrates a beautiful click effect using Heroicons and particle animation. When users click anywhere on the page, heart icons will appear and animate with a particle effect.

## Live Demo
Experience the click effect live at: [clickeffects.pages.dev](https://clickeffects.pages.dev)

## Screenshot
<img src="./public/DEMO1.gif" alt="示例图片" style="width:400px;height:400px;">


## Features
- **Particle Animation**: Heart icons animate with random velocity and fade out
- **Customizable Effects**: Adjustable parameters for particle size, speed, and colors
- **Responsive Design**: Works seamlessly across different screen sizes
- **Heroicons Integration**: Uses high-quality SVG icons from Heroicons library

## Technologies Used
- Next.js 15.1.0
- React 19
- TypeScript
- Heroicons
- Cloudflare Pages (for deployment)

## Getting Started

### Prerequisites
- Node.js (version 18 or higher)
- npm (version 9 or higher)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/clickeffects.git
   ```
2. Navigate to the project directory:
   ```bash
   cd clickeffects
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

### Running the Development Server
```

npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.

### Building for Production
```

npm run build
```

### Deployment
This project is configured for deployment on Cloudflare Pages. To deploy:
```

npm run deploy
```

## Configuration
The click effect can be customized by modifying the `DEFAULT_CONFIG` in `components/ClickEffect.tsx`:
```

const DEFAULT_CONFIG = {
  radius: 100,        // Spread radius of particles
  minSize: 10,        // Minimum particle size
  maxSize: 30,        // Maximum particle size
  colors: [           // Array of particle colors
    '#FFCCE1', 
    '#E195AB', 
    '#FFF5D7', 
    '#F2F9FF', 
    '#FFCCE1', 
    '#FFCCE1'
  ],
  speedFactor: 1      // Animation speed multiplier
};
```

## Project Structure
```

/clickeffects
├── components/          # React components
│   └── ClickEffect.tsx  # Main click effect component
├── app/                 # Next.js app directory
│   ├── page.tsx         # Main page
│   └── layout.tsx       # Root layout
├── public/              # Static assets
├── styles/              # CSS modules
├── next.config.ts       # Next.js configuration
├── package.json         # Project dependencies
└── README.md            # This file
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeatureName`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeatureName`)
5. Open a pull request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Heroicons](https://heroicons.com/) for the beautiful icons
- [Next.js](https://nextjs.org/) for the framework
- [Cloudflare Pages](https://pages.cloudflare.com/) for deployment