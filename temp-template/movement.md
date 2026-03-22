
```tsx
<style>
   #Yugo-45-prednji {
      visibility: hidden;
      animation: driveLeftToRight 5s linear infinite;
      animation-fill-mode: forwards;
    }

    #Yugo-45-daleki {
      visibility: hidden;
      animation: driveRightToLeft 6s linear infinite;
      animation-delay: 5s;
    }

    #wheel-blizi-auto-back,
    #wheel-blizi-auto-front {
      animation: spinWheel 0.5s linear infinite;
      transform-origin: center;
      transform-box: fill-box;
    }

    #wheel-daleki-auto-back,
    #wheel-daleki-auto-front {
      animation: spinWheel 0.5s linear infinite;
      animation-direction: reverse;
      transform-origin: center;
      transform-box: fill-box;
    }

    @keyframes spinWheel {
      from { transform: rotate(0deg); }
      to   { transform: rotate(360deg); }
    }

    @keyframes driveLeftToRight {
      from { visibility: visible; transform: translateX(-1400px); }
      to   { transform: translateX(1400px); }
    }

    @keyframes driveRightToLeft {
      from { visibility: visible; transform: translateX(1400px); }
      to   { transform: translateX(-1400px); }
    }
  </style>

```