<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Calendar Cop — Youth‑Activity Conflict Solver</title>
  <meta name="description" content="Paste your calendars, see conflicts, fix them in one click. Built for busy parents juggling kids' sports, school, and life." />
  <meta property="og:title" content="Calendar Cop — Youth‑Activity Conflict Solver" />
  <meta property="og:description" content="Paste your calendars, see conflicts, fix them in one click. Built for busy parents." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="https://dummyimage.com/1200x630/0f172a/ffffff&text=Calendar+Cop" />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='0.9em' font-size='90'>📆</text></svg>">
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .glass { backdrop-filter: blur(8px); background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03)); }
    .check:before { content: "✔"; }
  </style>
</head>
<body class="bg-slate-950 text-slate-100">
  <!-- Nav -->
  <header class="sticky top-0 z-30 border-b border-white/10 bg-slate-950/70 glass">
    <div class="mx-auto max-w-7xl px-4 py-3 flex items-center justify-between">
      <div class="flex items-center gap-2">
        <span class="text-2xl">📆</span>
        <span class="font-bold tracking-tight">Calendar Cop</span>
      </div>
      <nav class="hidden sm:flex items-center gap-6 text-sm text-slate-300">
        <a href="#how" class="hover:text-white">How it works</a>
        <a href="#features" class="hover:text-white">Features</a>
        <a href="#faq" class="hover:text-white">FAQ</a>
      </nav>
      <a href="#waitlist" class="rounded-xl bg-cyan-400/20 px-3 py-1.5 text-cyan-200 ring-1 ring-cyan-400/40 hover:bg-cyan-400/30">Join waitlist</a>
    </div>
  </header>

  <!-- Hero -->
  <section class="relative overflow-hidden">
    <div class="absolute inset-0 -z-10 bg-[radial-gradient(80rem_30rem_at_50%_-10%,rgba(6,182,212,.25),transparent_60%)]"></div>
    <div class="mx-auto max-w-7xl px-4 py-20 md:py-28 grid lg:grid-cols-2 gap-10 items-center">
      <div>
        <h1 class="text-4xl md:text-5xl font-black leading-tight tracking-tight">Stop schedule chaos.<br/>Detect <span class="text-cyan-300">youth‑activity conflicts</span> in seconds.</h1>
        <p class="mt-4 text-lg text-slate-300">Paste your calendars. We flag overlaps, travel‑time crunches, and kid‑specific double‑books — then give you one‑click fixes.</p>
        <ul class="mt-6 space-y-2 text-slate-200">
          <li class="flex gap-2"><span>✅</span><span>Games vs practices ranked by your priorities</span></li>
          <li class="flex gap-2"><span>✅</span><span>Travel‑time aware conflicts (not just busy/busy)</span></li>
          <li class="flex gap-2"><span>✅</span><span>One‑click carpool + coach templates</span></li>
        </ul>
        <form id="hero-form" class="mt-8 flex flex-col sm:flex-row gap-3" action="https://formspree.io/f/your-id" method="POST">
          <input required type="email" name="email" placeholder="you@email.com" class="w-full rounded-xl bg-white/5 px-4 py-3 ring-1 ring-white/10 focus:outline-none focus:ring-cyan-400 placeholder:text-slate-400" />
          <button class="rounded-xl bg-cyan-400 px-5 py-3 font-semibold text-slate-900 hover:bg-cyan-300">Join the waitlist</button>
        </form>
        <p class="mt-2 text-xs text-slate-400">No spam. Early users get lifetime 50% off.</p>
      </div>
      <div class="glass rounded-2xl border border-white/10 p-6 shadow-2xl">
        <div class="grid grid-cols-6 gap-2 text-xs">
          <!-- Faux calendar heat / demo -->
          <div class="col-span-6 font-semibold text-slate-300 mb-2">This week</div>
          <div class="col-span-6 grid grid-cols-7 gap-2">
            <div class="text-slate-400">Mon</div>
            <div class="text-slate-400">Tue</div>
            <div class="text-slate-400">Wed</div>
            <div class="text-slate-400">Thu</div>
            <div class="text-slate-400">Fri</div>
            <div class="text-slate-400">Sat</div>
            <div class="text-slate-400">Sun</div>
          </div>
          <div class="col-span-6 grid grid-cols-7 gap-2 mt-1">
            <!-- Fake blocks -->
            <div class="h-24 rounded-lg bg-white/5"></div>
            <div class="h-24 rounded-lg bg-white/5 ring-2 ring-yellow-400/60"></div>
            <div class="h-24 rounded-lg bg-white/5"></div>
            <div class="h-24 rounded-lg bg-white/5 ring-2 ring-red-500/70 relative">
              <span class="absolute -top-2 -right-2 rounded-full bg-red-500 px-2 py-0.5 text-[10px] font-bold">CONFLICT</span>
            </div>
            <div class="h-24 rounded-lg bg-white/5"></div>
            <div class="h-24 rounded-lg bg-white/5 ring-2 ring-yellow-400/60"></div>
            <div class="h-24 rounded-lg bg-white/5"></div>
          </div>
        </div>
        <div class="mt-4 rounded-xl bg-slate-900/60 p-4 text-sm text-slate-300">
          <p class="font-semibold">Example explanation</p>
          <p class="mt-1">Emma’s practice (5:30–6:30 @ West Field) overlaps with Jake’s game (6:00–7:00 @ East Rink). Drive time ~22 min. You’re short by 12 min.</p>
          <div class="mt-3 flex flex-wrap gap-2">
            <button class="rounded-lg bg-white/10 px-3 py-1.5 hover:bg-white/15">Ask for carpool</button>
            <button class="rounded-lg bg-white/10 px-3 py-1.5 hover:bg-white/15">Coach heads‑up</button>
            <button class="rounded-lg bg-white/10 px-3 py-1.5 hover:bg-white/15">Propose reschedule</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- How it works -->
  <section id="how" class="py-16 md:py-24 border-t border-white/10">
    <div class="mx-auto max-w-7xl px-4">
      <h2 class="text-3xl md:text-4xl font-extrabold">How it works</h2>
      <div class="mt-8 grid md:grid-cols-3 gap-6">
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <div class="text-2xl">1️⃣</div>
          <h3 class="mt-2 text-xl font-bold">Paste calendars</h3>
          <p class="mt-1 text-slate-300">Add iCal/ICS links from TeamSnap, TeamLinkt, GameChanger, Google/Outlook, or upload .ics files.</p>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <div class="text-2xl">2️⃣</div>
          <h3 class="mt-2 text-xl font-bold">We detect conflicts</h3>
          <p class="mt-1 text-slate-300">Time overlaps + travel‑buffer crunches per kid. Clear, human‑readable explanations.</p>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <div class="text-2xl">3️⃣</div>
          <h3 class="mt-2 text-xl font-bold">One‑click fixes</h3>
          <p class="mt-1 text-slate-300">Send carpool asks, coach messages, or reschedule suggestions instantly.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Features / Value -->
  <section id="features" class="py-16 md:py-24 border-t border-white/10">
    <div class="mx-auto max-w-7xl px-4">
      <h2 class="text-3xl md:text-4xl font-extrabold">Built for real life</h2>
      <div class="mt-8 grid md:grid-cols-2 gap-6">
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-xl font-bold">Family‑first logic</h3>
          <ul class="mt-3 space-y-2 text-slate-300">
            <li class="flex gap-2"><span>•</span><span>Set priorities: Games > Practices; Recitals > Practice</span></li>
            <li class="flex gap-2"><span>•</span><span>Per‑kid views and rules</span></li>
            <li class="flex gap-2"><span>•</span><span>Travel‑time buffers you control</span></li>
          </ul>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-xl font-bold">Concierge‑level fixes</h3>
          <ul class="mt-3 space-y-2 text-slate-300">
            <li class="flex gap-2"><span>•</span><span>Prewritten DM/email/SMS templates</span></li>
            <li class="flex gap-2"><span>•</span><span>Weekly conflict digest (PDF/email)</span></li>
            <li class="flex gap-2"><span>•</span><span>Coach & team‑friendly formatting</span></li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Social Proof / Testimonials -->
  <section class="py-16 md:py-24 border-t border-white/10">
    <div class="mx-auto max-w-7xl px-4">
      <h2 class="text-3xl md:text-4xl font-extrabold">What parents say</h2>
      <div class="mt-8 grid md:grid-cols-3 gap-6">
        <figure class="rounded-2xl border border-white/10 p-6 glass text-slate-300">
          <blockquote>“We caught three conflicts for Saturday before breakfast. No more scramble‑texting at 5pm.”</blockquote>
          <figcaption class="mt-3 text-slate-400">— Kayla, 2 kids, soccer & dance</figcaption>
        </figure>
        <figure class="rounded-2xl border border-white/10 p-6 glass text-slate-300">
          <blockquote>“The coach template saved me from writing awkward messages. 30 seconds and done.”</blockquote>
          <figcaption class="mt-3 text-slate-400">— Marcus, hockey dad</figcaption>
        </figure>
        <figure class="rounded-2xl border border-white/10 p-6 glass text-slate-300">
          <blockquote>“It respects travel time. That’s the missing piece other calendars ignore.”</blockquote>
          <figcaption class="mt-3 text-slate-400">— Priya, piano & swim</figcaption>
        </figure>
      </div>
    </div>
  </section>

  <!-- CTA / Waitlist -->
  <section id="waitlist" class="py-16 md:py-24 border-t border-white/10">
    <div class="mx-auto max-w-3xl px-4 text-center">
      <h2 class="text-3xl md:text-4xl font-extrabold">Be first. Get 50% off for life.</h2>
      <p class="mt-3 text-slate-300">We’re inviting early parents, coaches, and leagues. Drop your email and we’ll send the private beta.</p>
      <form id="cta-form" class="mt-6 flex flex-col sm:flex-row gap-3 justify-center" action="https://formspree.io/f/your-id" method="POST">
        <input required type="email" name="email" placeholder="you@email.com" class="w-full sm:w-80 rounded-xl bg-white/5 px-4 py-3 ring-1 ring-white/10 focus:outline-none focus:ring-cyan-400 placeholder:text-slate-400" />
        <button class="rounded-xl bg-cyan-400 px-5 py-3 font-semibold text-slate-900 hover:bg-cyan-300">Join the waitlist</button>
      </form>
      <p class="mt-2 text-xs text-slate-500">By joining, you agree to our <a href="#" class="underline hover:text-slate-300">privacy policy</a>.</p>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq" class="py-16 md:py-24 border-t border-white/10">
    <div class="mx-auto max-w-5xl px-4">
      <h2 class="text-3xl md:text-4xl font-extrabold">FAQ</h2>
      <div class="mt-8 grid md:grid-cols-2 gap-6">
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-lg font-bold">Is this a full calendar app?</h3>
          <p class="mt-2 text-slate-300">No. It’s a <em>conflict solver</em>. We focus on detecting and resolving overlaps better than generic calendars.</p>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-lg font-bold">How do I add my schedules?</h3>
          <p class="mt-2 text-slate-300">Paste iCal/ICS links (TeamSnap, TeamLinkt, Google/Outlook, school sites) or upload .ics files.</p>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-lg font-bold">What’s pricing?</h3>
          <p class="mt-2 text-slate-300">Target: $7/mo family, $49/yr. League dashboards available in beta.</p>
        </div>
        <div class="rounded-2xl border border-white/10 p-6 glass">
          <h3 class="text-lg font-bold">When is the beta?</h3>
          <p class="mt-2 text-slate-300">We’re onboarding in waves. Join the waitlist and we’ll email you an invite.</p>
        </div>
      </div>
    </div>
  </section>

  <footer class="border-t border-white/10 py-10 text-center text-sm text-slate-400">
    <div class="mx-auto max-w-7xl px-4">
      <p>© <span id="y"></span> Calendar Cop. All rights reserved.</p>
      <p class="mt-1">Made for busy families — especially solo parents.</p>
    </div>
  </footer>

  <!-- Lightweight analytics placeholder -->
  <!-- Replace with Plausible/GA as needed -->
  <script>
    document.getElementById('y').textContent = new Date().getFullYear();

    // Optional: Mailto fallback if you don't want Formspree yet
    for (const form of [document.getElementById('hero-form'), document.getElementById('cta-form')]) {
      form?.addEventListener('submit', (e) => {
        const hasFormspree = form.action.includes('/f/your-id') === false;
        if (!hasFormspree) {
          e.preventDefault();
          const email = form.querySelector('input[type="email"]').value;
          window.location.href = `mailto:hello@calendarcop.app?subject=Waitlist&body=${encodeURIComponent(email)}`;
        }
      });
    }
  </script>
</body>
</html>
