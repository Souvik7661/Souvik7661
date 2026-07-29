<svg viewBox="0 0 900 260" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="panelGlow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="2" result="b"/>
      <feMerge>
        <feMergeNode in="b"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <pattern id="dotGrid2" width="26" height="26" patternUnits="userSpaceOnUse">
      <circle cx="1.2" cy="1.2" r="1.2" fill="#152242"/>
    </pattern>
  </defs>

  <rect width="900" height="260" rx="14" fill="#060a1a"/>
  <rect width="900" height="260" rx="14" fill="url(#dotGrid2)"/>
  <rect x="1.5" y="1.5" width="897" height="257" rx="13" fill="none" stroke="#1e2a4a" stroke-width="2"/>

  <!-- status LEDs: sequential handshake, not a decoration -->
  <g font-family="JetBrains Mono, monospace" font-size="11" fill="#64748B">
    <circle cx="34" cy="32" r="6" fill="#00F7FF" filter="url(#panelGlow)">
      <animate attributeName="opacity" values="0.3;1;0.3" dur="1.8s" begin="0s" repeatCount="indefinite"/>
    </circle>
    <text x="48" y="36">PWR</text>

    <circle cx="110" cy="32" r="6" fill="#2563EB" filter="url(#panelGlow)">
      <animate attributeName="opacity" values="0.3;1;0.3" dur="1.8s" begin="0.4s" repeatCount="indefinite"/>
    </circle>
    <text x="124" y="36">NET</text>

    <circle cx="186" cy="32" r="6" fill="#7C3AED" filter="url(#panelGlow)">
      <animate attributeName="opacity" values="0.3;1;0.3" dur="1.8s" begin="0.8s" repeatCount="indefinite"/>
    </circle>
    <text x="200" y="36">SYS</text>
  </g>

  <line x1="24" y1="54" x2="560" y2="54" stroke="#1e2a4a" stroke-width="1.5"/>

  <!-- boot log: revealed line by line -->
  <g font-family="JetBrains Mono, monospace" font-size="15" fill="#94A3B8">
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.15s" begin="0.3s" fill="freeze"/>
      <text x="24" y="82">INIT   kernel............<tspan fill="#10B981">OK</tspan></text></g>
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.15s" begin="0.6s" fill="freeze"/>
      <text x="24" y="107">MOUNT  java_runtime.......<tspan fill="#10B981">OK</tspan></text></g>
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.15s" begin="0.9s" fill="freeze"/>
      <text x="24" y="132">MOUNT  python_env.........<tspan fill="#10B981">OK</tspan></text></g>
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.15s" begin="1.2s" fill="freeze"/>
      <text x="24" y="157">LINK   ai_modules.........<tspan fill="#10B981">OK</tspan></text></g>
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.15s" begin="1.5s" fill="freeze"/>
      <text x="24" y="182">BUILD  ambition...........<tspan fill="#10B981">OK</tspan></text></g>
    <g opacity="0"><animate attributeName="opacity" from="0" to="1" dur="0.2s" begin="1.9s" fill="freeze"/>
      <text x="24" y="212" font-weight="700" fill="#00F7FF">STATUS: READY — OPEN TO INTERNSHIPS</text></g>
  </g>
  <rect x="24" y="218" width="10" height="16" fill="#00F7FF">
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" begin="2.1s" repeatCount="indefinite"/>
  </rect>

  <!-- activity equalizer: system load readout -->
  <line x1="600" y1="54" x2="876" y2="54" stroke="#1e2a4a" stroke-width="1.5"/>
  <text x="600" y="36" font-family="JetBrains Mono, monospace" font-size="11" fill="#64748B">SYSTEM LOAD</text>

  <g fill="#06B6D4">
    <rect x="612" y="170" width="16" height="40"><animate attributeName="height" values="40;110;60;90;40" dur="2.1s" repeatCount="indefinite"/><animate attributeName="y" values="170;100;150;120;170" dur="2.1s" repeatCount="indefinite"/></rect>
    <rect x="642" y="150" width="16" height="60"><animate attributeName="height" values="60;30;100;50;60" dur="1.7s" repeatCount="indefinite"/><animate attributeName="y" values="150;180;110;160;150" dur="1.7s" repeatCount="indefinite"/></rect>
    <rect x="672" y="120" width="16" height="90"><animate attributeName="height" values="90;120;40;100;90" dur="2.4s" repeatCount="indefinite"/><animate attributeName="y" values="120;90;170;110;120" dur="2.4s" repeatCount="indefinite"/></rect>
    <rect x="702" y="140" width="16" height="70"><animate attributeName="height" values="70;100;50;120;70" dur="1.9s" repeatCount="indefinite"/><animate attributeName="y" values="140;110;160;90;140" dur="1.9s" repeatCount="indefinite"/></rect>
    <rect x="732" y="160" width="16" height="50"><animate attributeName="height" values="50;90;110;60;50" dur="2.2s" repeatCount="indefinite"/><animate attributeName="y" values="160;120;100;150;160" dur="2.2s" repeatCount="indefinite"/></rect>
    <rect x="762" y="130" width="16" height="80"><animate attributeName="height" values="80;50;100;70;80" dur="1.6s" repeatCount="indefinite"/><animate attributeName="y" values="130;160;110;140;130" dur="1.6s" repeatCount="indefinite"/></rect>
    <rect x="792" y="150" width="16" height="60"><animate attributeName="height" values="60;100;40;90;60" dur="2.0s" repeatCount="indefinite"/><animate attributeName="y" values="150;110;170;120;150" dur="2.0s" repeatCount="indefinite"/></rect>
    <rect x="822" y="170" width="16" height="40"><animate attributeName="height" values="40;80;110;50;40" dur="2.3s" repeatCount="indefinite"/><animate attributeName="y" values="170;130;100;160;170" dur="2.3s" repeatCount="indefinite"/></rect>
  </g>
  <line x1="600" y1="210" x2="876" y2="210" stroke="#1e2a4a" stroke-width="1.5"/>
</svg>
