<script>
  import { onMount } from 'svelte';

  const images = [
    "/generated/image-live-concert-performance-with-stage-ligh-1765659197349-0.webp",
    "/generated/image-conference-speaker-presenting-on-stage-t-1765659200047-1.webp",
    "/generated/image-music-festival-outdoor-stage-with-crowd--1765659202281-2.webp",
    "/generated/image-event-organizer-working-on-laptop-at-ven-1765659204644-3.webp",
    "/generated/image-live-streaming-production-setup-with-cam-1765659207072-4.webp"
  ];

  const floatingImages = {
    venue: "/generated/image-event-venue-manager-confidently-overseei-1765659209360-5.webp",
    audience: "/generated/image-audience-members-watching-and-engaging-w-1765659211669-6.webp",
    theater: "/generated/image-theater-performance-with-dramatic-lighti-1765659213920-7.webp",
    concert: "/generated/image-live-concert-performance-with-stage-ligh-1765659197349-0.webp",
    conference: "/generated/image-conference-speaker-presenting-on-stage-t-1765659200047-1.webp"
  };

  let showCookieBanner = $state(true);
</script>

<div class="font-sans text-[#111] antialiased bg-white selection:bg-black selection:text-white">
  <!-- Header -->
  <header class="fixed top-0 left-0 w-full z-50 flex justify-between items-center px-6 py-5 bg-white/90 backdrop-blur-sm">
    <div class="flex items-center gap-3">
      <svg width="80" height="28" viewBox="0 0 1935 655" xmlns="http://www.w3.org/2000/svg">
        <path fill="#EF0000" d="M819.000000,1.000000 C916.020935,1.000000 1013.041809,1.000000 1110.661743,1.367424 C1112.172363,3.106959 1113.762817,4.420705 1113.886719,5.860521 C1114.760010,16.018583 1115.378784,26.199757 1115.987671,36.379002 C1116.705688,48.385098 1117.336426,60.396446 1117.996826,72.405960 C1119.001343,90.669388 1119.996338,108.933350 1121.000732,127.196800 C1121.661255,139.206268 1122.348389,151.214310 1122.992920,163.224640 C1124.008789,182.153870 1124.982056,201.085373 1126.006226,220.014130 C1126.638062,231.691971 1127.370850,243.364380 1127.987183,255.042999 C1129.021362,274.637604 1130.041626,294.233124 1130.981323,313.832367 C1131.424805,323.080139 1131.623657,332.339417 1132.018311,341.589844 C1132.263916,347.348267 1132.275757,353.163757 1133.196533,358.822815 C1133.560425,361.058746 1136.025146,364.535126 1137.677734,364.619507 C1140.362427,364.756653 1141.947021,362.021088 1142.082642,358.669250 C1142.528564,347.650787 1143.369995,336.648956 1143.987671,325.636688 C1144.698364,312.963623 1145.312622,300.285126 1146.005737,287.611023 C1146.644287,275.933502 1147.353149,264.259827 1147.992920,252.582382 C1149.011963,233.986557 1149.992188,215.388626 1151.002319,196.792313 C1151.654785,184.782379 1152.376953,172.776077 1152.985474,160.763962 C1153.703369,146.591705 1154.260864,132.411102 1155.024170,118.241440 C1155.563599,108.224518 1156.423340,98.224953 1156.974976,88.208549 C1158.044800,68.782623 1158.732544,49.331387 1160.112061,29.928566 C1160.800903,20.242533 1162.666626,10.640188 1164.000000,0.999995 C1258.020874,1.000000 1352.041870,1.000000 1446.657471,1.363754 C1448.167969,3.430408 1449.810059,5.114679 1449.854248,6.839923 C1449.958740,10.909713 1449.377441,15.007149 1448.938965,19.078915 C1447.661499,30.939171 1446.250610,42.785362 1445.023804,54.650688 C1444.214233,62.482094 1443.744873,70.348869 1442.921387,78.178589 C1441.708618,89.712173 1440.229614,101.217850 1439.029663,112.752663 C1438.197998,120.747833 1437.750000,128.782562 1436.943726,136.780792 C1435.714111,148.979370 1434.275269,161.156754 1433.017456,173.352646 C1432.243896,180.854095 1431.718628,188.381134 1430.945801,195.882675 C1429.689209,208.078552 1428.274536,220.258148 1427.017090,232.453964 C1426.243652,239.955551 1425.719360,247.482895 1424.939697,254.983749 C1423.689087,267.013519 1422.262817,279.025055 1421.020508,291.055603 C1420.228760,298.722076 1419.729248,306.418823 1418.931152,314.084564 C1417.695923,325.949127 1416.250366,337.791870 1415.023560,349.657257 C1414.213623,357.488556 1413.743530,365.355225 1412.920166,373.184906 C1411.707520,384.718536 1410.229126,396.224335 1409.029663,407.759216 C1408.198120,415.754425 1407.749634,423.789124 1406.943359,431.787384 C1405.713623,443.985901 1404.275269,456.163330 1403.017456,468.359192 C1402.243896,475.860657 1401.718262,483.387665 1400.945190,490.889191 C1399.688599,503.085022 1398.274414,515.264648 1397.017212,527.460449 C1396.243896,534.962097 1395.748413,542.492920 1394.932007,549.989319 C1393.712280,561.189575 1392.204590,572.358887 1391.038086,583.564209 C1390.171387,591.888733 1389.765015,600.260559 1388.951294,608.591553 C1387.726929,621.123779 1386.551636,633.668396 1384.913574,646.149780 C1383.954346,653.459595 1384.259766,655.034424 1375.369873,655.031982 C1216.875122,654.987976 1058.380371,654.999939 899.885559,654.999695 C898.552307,654.999695 897.185608,655.185791 895.892395,654.957397 C892.804077,654.412048 890.140747,653.623657 889.907471,649.479614 C889.559509,643.297302 888.696899,637.139954 887.943115,630.985474 C886.674316,620.625916 885.243408,610.285889 884.026306,599.920532 C883.205261,592.927368 882.732971,585.893555 881.928711,578.898071 C880.698914,568.201294 879.253296,557.529358 878.022827,546.832581 C877.218079,539.837036 876.748413,532.802673 875.920105,525.810364 C874.711731,515.610840 873.204529,505.446289 872.031372,495.243103 C870.872192,485.161835 870.057190,475.041229 868.930908,464.955811 C867.717590,454.090759 866.266235,443.252411 865.018860,432.390961 C864.234375,425.559875 863.741943,418.694763 862.925659,411.867950 C861.706299,401.669586 860.204895,391.504364 859.031738,381.301117 C857.872681,371.220367 857.060669,361.099945 855.934387,351.015015 C854.720947,340.149872 853.266907,329.311798 852.019165,318.450256 C851.234375,311.618896 850.751343,304.752136 849.926636,297.926208 C848.714478,287.893402 847.188599,277.897736 846.036377,267.858704 C844.860413,257.613220 844.064026,247.324600 842.936890,237.072952 C841.724121,226.041138 840.279053,215.035049 839.015137,204.008606 C838.250916,197.341629 837.745178,190.644226 836.932922,183.983719 C835.709534,173.952011 834.188965,163.955627 833.036560,153.916473 C831.860474,143.671066 831.066833,133.382233 829.939758,123.130661 C828.726868,112.098808 827.289368,101.091843 826.011475,90.066879 C825.220398,83.242310 824.610535,76.396545 823.800354,69.574417 C822.588440,59.369308 821.284912,49.174988 819.995728,38.979187 C819.034668,31.378571 817.497864,23.800825 817.242920,16.178591 C817.075562,11.175309 814.061035,5.511446 819.000000,1.000000 z"/>
        <path fill="#EF0000" d="M1676.000000,1.000004 C1762.570068,1.000000 1849.140259,1.000000 1936.000000,1.000000 C1936.000000,45.020470 1936.000000,89.041580 1935.531372,133.531342 C1882.143799,134.000000 1829.224731,134.000000 1776.282593,134.000000 C1776.282593,149.932922 1776.282593,165.329376 1776.282593,181.147278 C1823.619995,181.147278 1870.676392,181.147278 1917.710083,181.147278 C1917.710083,226.961182 1917.710083,272.349854 1917.710083,318.161865 C1870.365356,318.161865 1823.308960,318.161865 1776.308472,318.161865 C1776.308472,333.985260 1776.308472,349.382233 1776.308472,365.000000 C1829.744385,365.000000 1882.872192,365.000000 1936.000000,365.000000 C1936.000000,461.944153 1936.000000,558.888306 1936.000000,656.000000 C1779.979126,656.000000 1623.958130,656.000000 1467.468628,655.531372 C1467.000000,437.428192 1467.000000,219.793686 1467.000000,2.000000 C1469.503540,2.000000 1471.324951,2.000000 1473.146484,2.000000 C1538.944824,2.000000 1604.743164,2.008021 1670.541504,1.958094 C1672.361206,1.956713 1674.180542,1.333342 1676.000000,1.000004 z"/>
      </svg>
    </div>
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium">
      <a href="#platform" class="hover:opacity-70 transition-opacity">Platform</a>
      <a href="#features" class="hover:opacity-70 transition-opacity">Features</a>
      <a href="#pricing" class="hover:opacity-70 transition-opacity">Pricing</a>
      <a href="#contact" class="hover:opacity-70 transition-opacity">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="pt-40 pb-20 px-6 max-w-[1400px] mx-auto">
    <div class="max-w-4xl mb-24">
      <h1 class="text-6xl md:text-7xl font-medium tracking-tight leading-[1.1] mb-8">
        Instant video commerce<br>for live events
      </h1>
      <div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-8">
        <p class="text-lg md:text-xl max-w-md leading-relaxed text-gray-800">
          Real-time streaming infrastructure that converts viewers into buyers. No technical expertise required.
        </p>
        <button class="bg-[#EF0000] text-white px-6 py-3 text-sm font-medium rounded-sm hover:bg-[#d00000] transition-colors">
          Get started
        </button>
      </div>
    </div>

    <!-- Hero Images Grid -->
    <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
      {#each images as src, i}
        <div class="aspect-[3/4] overflow-hidden bg-gray-100 rounded-sm">
          <img {src} alt="Live event streaming {i}" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
        </div>
      {/each}
    </div>
  </section>

  <!-- Floating Images Section -->
  <section class="py-32 px-6 max-w-[1400px] mx-auto relative min-h-[800px]">
    <div class="absolute inset-0 flex items-center justify-center pointer-events-none z-10">
      <h2 class="text-2xl md:text-3xl font-medium text-center max-w-2xl leading-snug bg-white/80 backdrop-blur-sm p-4 rounded-xl">
        Stream any live event with guaranteed 99.9% uptime. Turn every viewer into a potential customer.
      </h2>
    </div>

    <!-- Scattered Images with 'Go Live' -->
    <div class="relative w-full h-full min-h-[800px]">
      <!-- Image 1: Conference (Left) -->
      <div class="absolute top-20 left-[10%] w-64 aspect-[3/4]">
        <img src={floatingImages.conference} alt="Conference" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <div class="w-3 h-3 bg-[#EF0000] rounded-full mx-auto mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">● LIVE</button>
        </div>
      </div>

      <!-- Image 2: Venue Manager (Center Top) -->
      <div class="absolute top-0 left-[45%] w-56 aspect-video">
        <img src={floatingImages.venue} alt="Venue Manager" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/3 left-1/3">
             <div class="w-3 h-3 bg-[#EF0000] rounded-full mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">● LIVE</button>
        </div>
      </div>

       <!-- Image 3: Audience (Right Top) -->
      <div class="absolute top-40 right-[5%] w-80 aspect-video">
        <img src={floatingImages.audience} alt="Audience Engagement" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute bottom-1/3 right-1/3">
             <div class="w-3 h-3 bg-[#EF0000] rounded-full mb-2 animate-pulse ml-auto"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">● LIVE</button>
        </div>
      </div>

      <!-- Image 4: Concert (Left Bottom) -->
      <div class="absolute bottom-20 left-[5%] w-56 aspect-[3/4]">
        <img src={floatingImages.concert} alt="Concert" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">● LIVE</button>
        </div>
      </div>

      <!-- Image 5: Theater (Center Bottom) -->
      <div class="absolute bottom-0 left-[35%] w-48 aspect-[3/4]">
        <img src={floatingImages.theater} alt="Theater" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">● LIVE</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 1: Real-Time Production -->
  <section class="bg-[#111] text-white py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight max-w-xl">
          Real-time production<br>tools that just work
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Professional-grade streaming infrastructure designed for event organizers. No technical expertise or expensive equipment needed.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-video bg-[#1a1a1a] rounded-sm mb-16 flex items-center justify-center relative overflow-hidden group">
        <div class="flex items-center gap-4">
          <div class="w-4 h-4 bg-[#EF0000] rounded-full animate-pulse"></div>
          <div class="text-5xl md:text-7xl font-light tracking-tight text-white/90">
            LIVE
          </div>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 border-t border-white/10 pt-12">
        <div>
          <h3 class="text-lg font-medium mb-3">One-click streaming</h3>
          <p class="text-gray-400 leading-relaxed">Go live instantly from any venue without complex setup.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Built-in commerce</h3>
          <p class="text-gray-400 leading-relaxed">Convert viewers into buyers with integrated payment flows.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Enterprise reliability</h3>
          <p class="text-gray-400 leading-relaxed">99.9% uptime SLA ensures your stream never drops.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 2: Scale to 10M Streams -->
  <section class="bg-[#111] text-white py-32 px-6 border-t border-white/5">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight">
          Built to scale with<br>your ambitions
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          From intimate venues to massive festivals. Our infrastructure handles 10M+ concurrent streams without breaking a sweat.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-[2/1] bg-[#1a1a1a] rounded-sm flex items-center justify-center">
         <div class="text-5xl md:text-7xl font-light tracking-tight text-white/90">
          10M<span class="text-[#EF0000]">+</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Light Gray Section -->
  <section class="bg-[#f5f5f5] py-24 px-6">
    <div class="max-w-[1400px] mx-auto grid grid-cols-1 md:grid-cols-3 gap-12">
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Zero technical barriers</h3>
        <p class="text-gray-600 leading-relaxed">No engineering team or expensive equipment required.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Guaranteed reliability</h3>
        <p class="text-gray-600 leading-relaxed">99.9% uptime SLA backed by enterprise infrastructure.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Instant monetization</h3>
        <p class="text-gray-600 leading-relaxed">Turn viewers into buyers with seamless commerce integration.</p>
      </div>
    </div>
  </section>

  <!-- Built for Live Entertainment -->
  <section class="bg-[#f0f0f0] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="mb-16">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-6 text-[#111]">
          Capturing the $100B live<br>entertainment market
        </h2>
        <p class="text-gray-600 text-lg max-w-2xl leading-relaxed">
          3LIVE empowers event creators to monetize their content through seamless streaming and commerce integration. From concerts to conferences, we handle the technical complexity so you can focus on your audience.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Visual -->
        <div class="bg-[#111] aspect-video rounded-xl flex items-center justify-center relative overflow-hidden perspective-1000">
           <!-- Abstract Streaming Animation -->
           <div class="relative w-64 h-40 flex items-center justify-center transform-style-3d">
              {#each [0, 1, 2, 3, 4] as i}
                <div 
                  class="absolute w-32 h-48 border border-white/30 bg-white/5 backdrop-blur-sm rounded-sm transition-transform duration-500"
                  style="
                    transform: translateX({(i - 2) * 40}px) translateZ({Math.abs(i - 2) * -20}px) rotateY({(i - 2) * 10}deg);
                    z-index: {10 - Math.abs(i - 2)};
                  "
                ></div>
              {/each}
              <!-- Central Highlight with red accent -->
              <div class="absolute w-32 h-48 border border-[#EF0000]/60 shadow-[0_0_15px_rgba(239,0,0,0.3)] rounded-sm z-20"></div>
           </div>
        </div>

        <!-- List -->
        <div class="space-y-12 pt-4">
          <div class="group cursor-pointer">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Seamless venue integration</h3>
            <p class="text-gray-600 leading-relaxed">Works with any venue setup. No complicated installations or dedicated IT staff required.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Real-time analytics</h3>
            <p class="text-gray-600 leading-relaxed">Track viewer engagement, conversion rates, and revenue in real-time during your events.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Multi-platform distribution</h3>
            <p class="text-gray-600 leading-relaxed">Stream simultaneously to multiple platforms while maintaining full control and monetization.</p>
          </div>

          <div class="flex gap-4 pt-8">
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">←</button>
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">→</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fast to Launch -->
  <section class="bg-[#fffcf8] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-20 text-[#111]">
        Go live in minutes,<br>not months
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
        <!-- Card 1 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Instant setup</h3>
          <p class="text-gray-600 leading-relaxed">Start streaming your first event in under 10 minutes. No technical knowledge required.</p>
        </div>

        <!-- Card 2 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75 11.25 15 15 9.75m-3-7.036A11.959 11.959 0 0 1 3.598 6 11.99 11.99 0 0 0 3 9.749c0 5.592 3.824 10.29 9 11.623 5.176-1.332 9-6.03 9-11.622 0-1.31-.21-2.571-.598-3.751h-.152c-3.196 0-6.1-1.248-8.25-3.285Z" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Enterprise reliability</h3>
          <p class="text-gray-600 leading-relaxed">99.9% uptime SLA ensures your streams are always available when it matters.</p>
        </div>

        <!-- Card 3 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 18.75a60.07 60.07 0 0 1 15.797 2.101c.727.198 1.453-.342 1.453-1.096V18.75M3.75 4.5v.75A.75.75 0 0 1 3 6h-.75m0 0v-.375c0-.621.504-1.125 1.125-1.125H20.25M2.25 6v9m18-10.5v.75c0 .414.336.75.75.75h.75m-1.5-1.5h.375c.621 0 1.125.504 1.125 1.125v9.75c0 .621-.504 1.125-1.125 1.125h-.375m1.5-1.5H21a.75.75 0 0 0-.75.75v.75m0 0H3.75m0 0h-.375a1.125 1.125 0 0 1-1.125-1.125V15m1.5 1.5v-.75A.75.75 0 0 0 3 15h-.75M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm3 0h.008v.008H18V10.5Zm-12 0h.008v.008H6V10.5Z" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Built-in monetization</h3>
          <p class="text-gray-600 leading-relaxed">Integrated payment processing turns every viewer into a potential customer.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Banner -->
  <section class="px-6 py-12">
    <div class="max-w-[1400px] mx-auto border border-gray-100 rounded-xl p-8 md:p-12 flex flex-col md:flex-row justify-between items-center gap-8 bg-white shadow-sm">
      <div class="flex items-center gap-6">
        <div class="flex gap-1 h-8">
           <div class="w-2 bg-[#EF0000] h-full"></div>
           <div class="w-2 bg-[#EF0000] h-full"></div>
           <div class="w-2 bg-[#EF0000] h-full"></div>
           <div class="w-2 bg-[#EF0000] h-full opacity-50"></div>
        </div>
        <h2 class="text-2xl md:text-3xl font-medium tracking-tight">Ready to transform your events?</h2>
      </div>
      <button class="bg-[#EF0000] text-white px-8 py-3 text-sm font-medium rounded-sm hover:bg-[#d00000] transition-colors whitespace-nowrap">
        Book a demo
      </button>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1400px] mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 md:gap-24 mb-20">
        <div class="col-span-1 md:col-span-2">
          <h3 class="text-xl font-medium mb-1">3LIVE</h3>
          <p class="text-gray-500 text-lg">Live Video Commerce</p>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="#" class="hover:underline">Contact Us</a></li>
            <li><a href="#" class="hover:underline">Platform</a></li>
            <li><a href="#" class="hover:underline">Pricing</a></li>
          </ul>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="#" class="hover:underline">LinkedIn</a></li>
            <li><a href="#" class="hover:underline">Twitter</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-end text-[10px] text-gray-400 uppercase tracking-wider gap-4">
        <div class="flex gap-8">
          <span>3LIVE 2025</span>
        </div>
        <div class="flex gap-8">
          <a href="#" class="hover:text-gray-600">Terms of use</a>
          <a href="#" class="hover:text-gray-600">Privacy Policy</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Cookie Banner -->
  {#if showCookieBanner}
    <div class="fixed bottom-6 right-6 max-w-sm bg-white border border-gray-100 shadow-xl p-6 rounded-sm z-50 text-xs text-gray-600">
      <p class="mb-4 leading-relaxed">
        We use cookies to improve your experience. See our <a href="#" class="underline text-black">Privacy Policy</a> for details.
      </p>
      <button onclick={() => showCookieBanner = false} class="bg-[#EF0000] text-white px-4 py-2 rounded-sm font-medium hover:bg-[#d00000] transition-colors">
        Accept
      </button>
    </div>
  {/if}
</div>

<style>
  :global(body) {
    font-family: 'Inter', sans-serif;
  }
  .perspective-1000 {
    perspective: 1000px;
  }
  .transform-style-3d {
    transform-style: preserve-3d;
  }
</style>

