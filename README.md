
<svg xmlns="http://www.w3.org/2000/svg" width="1500" height="500" viewBox="0 0 1500 500">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#050B18"/>
      <stop offset="55%" stop-color="#0A1730"/>
      <stop offset="100%" stop-color="#07101F"/>
    </linearGradient>

    <linearGradient id="cyan" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#00D9FF"/>
      <stop offset="100%" stop-color="#3987FF"/>
    </linearGradient>

    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M40 0H0V40" fill="none" stroke="#173253" stroke-width="1" opacity=".35"/>
    </pattern>

    <filter id="glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="1500" height="500" fill="url(#bg)"/>
  <rect width="1500" height="500" fill="url(#grid)"/>

  <!-- Ambient lighting -->
  <circle cx="1180" cy="180" r="260" fill="#087CFF" opacity=".08"/>
  <circle cx="250" cy="450" r="220" fill="#00D9FF" opacity=".05"/>

  <!-- Decorative circuit paths -->
  <g fill="none" stroke="url(#cyan)" stroke-width="2" opacity=".45">
    <path d="M0 95H160L195 130H310"/>
    <path d="M0 115H130L165 150H250"/>
    <path d="M1500 80H1360L1325 115H1230"/>
    <path d="M1500 105H1400L1360 145H1280"/>
    <path d="M1080 500V430L1120 390V330"/>
    <path d="M1150 500V455L1190 415V370"/>
  </g>

  <g fill="#00D9FF" filter="url(#glow)">
    <circle cx="310" cy="130" r="4"/>
    <circle cx="250" cy="150" r="4"/>
    <circle cx="1230" cy="115" r="4"/>
    <circle cx="1280" cy="145" r="4"/>
    <circle cx="1120" cy="330" r="4"/>
    <circle cx="1190" cy="370" r="4"/>
  </g>

  <!-- Terminal panel -->
  <g transform="translate(105 105)">
    <rect width="350" height="220" rx="12" fill="#080F1D" stroke="#24476C" stroke-width="1.5"/>
    <path d="M0 42H350" stroke="#24476C"/>
    <circle cx="22" cy="21" r="5" fill="#FF5F57"/>
    <circle cx="42" cy="21" r="5" fill="#FEBC2E"/>
    <circle cx="62" cy="21" r="5" fill="#28C840"/>

    <g font-family="Consolas, monospace" font-size="13">
      <text x="20" y="72" fill="#00D9FF">$ whoami</text>
      <text x="20" y="98" fill="#A9C7E8">developer</text>
      <text x="20" y="130" fill="#00D9FF">$ cat interests.txt</text>
      <text x="20" y="156" fill="#A9C7E8">software engineering</text>
      <text x="20" y="178" fill="#A9C7E8">backend · AI · systems</text>
      <text x="20" y="205" fill="#00D9FF">_</text>
    </g>
  </g>

  <!-- Code panel -->
  <g transform="translate(1120 175)">
    <rect width="275" height="190" rx="12" fill="#080F1D" stroke="#24476C" stroke-width="1.5"/>
    <path d="M0 40H275" stroke="#24476C"/>
    <g font-family="Consolas, monospace" font-size="12">
      <text x="18" y="26" fill="#7E9BBE">main.py</text>
      <text x="20" y="72" fill="#C792EA">def</text>
      <text x="52" y="72" fill="#82AAFF"> build_future</text>
      <text x="143" y="72" fill="#A9C7E8">():</text>
      <text x="35" y="98" fill="#C792EA">while</text>
      <text x="77" y="98" fill="#A9C7E8"> learning:</text>
      <text x="52" y="124" fill="#82AAFF">    build()</text>
      <text x="52" y="150" fill="#82AAFF">    improve()</text>
      <text x="20" y="176" fill="#00D9FF">▌</text>
    </g>
  </g>

  <!-- Main identity -->
  <g text-anchor="middle">
    <text x="750" y="225"
          font-family="Arial, Helvetica, sans-serif"
          font-size="48"
          font-weight="700"
          letter-spacing="3"
          fill="#F1F7FF">
      SAI RAM PRAGNEY
    </text>

    <text x="750" y="285"
          font-family="Arial, Helvetica, sans-serif"
          font-size="48"
          font-weight="700"
          letter-spacing="3"
          fill="url(#cyan)">
      MURIKIPUDI
    </text>

    <rect x="590" y="315" width="320" height="3" rx="2" fill="url(#cyan)" opacity=".9"/>
  </g>

  <!-- Bottom technical details -->
  <g fill="#426487" opacity=".8">
    <circle cx="520" cy="420" r="2"/>
    <circle cx="980" cy="420" r="2"/>
    <circle cx="550" cy="440" r="2"/>
    <circle cx="950" cy="440" r="2"/>
  </g>

  <path d="M0 475H1500" stroke="#173253" stroke-width="1"/>
  <path d="M0 475H400" stroke="url(#cyan)" stroke-width="2" opacity=".7"/>
</svg>
