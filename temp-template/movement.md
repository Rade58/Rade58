
```tsx
<style>
  #Yugo-45-prednji {
    visibility: hidden;
    animation: driveLeftToRight 5s linear infinite;
    animation-fill-mode: forwards;
  }

  #Yugo-45-daleki {
    visibility: hidden;
    animation: driveRightToLeft 8s linear infinite;
    animation-delay: 4s;
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

  #ship-komjuteski {
    animation: floatAcross 10s ease-in-out infinite alternate;
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

  @keyframes floatAcross {
    from { transform: translateX(0px); }
    to   { transform: translateX(-560px); }
  }
</style>

```