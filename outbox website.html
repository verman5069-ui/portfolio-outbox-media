import React, { useState, useEffect } from 'react';
import { 
  Play, 
  TrendingUp, 
  Users, 
  Video, 
  CheckCircle, 
  ArrowRight, 
  BarChart3, 
  Cpu, 
  Menu, 
  X, 
  Instagram, 
  Linkedin, 
  Mail,
  ChevronRight,
  Sparkles,
  Zap,
  Loader2
} from 'lucide-react';

// --- Brand Color Palette (Derived from Logo) ---
const brandColors = {
  bg: "bg-[#f9f9f9]", // Off-white background from logo
  teal: "text-[#006d5b]", 
  tealBg: "bg-[#006d5b]",
  blue: "text-[#0056b3]",
  blueBg: "bg-[#0056b3]",
  purple: "text-[#5e35b1]",
  purpleBg: "bg-[#5e35b1]",
  yellow: "text-[#fbc02d]",
  yellowBg: "bg-[#fbc02d]",
  dark: "text-[#1a1a1a]",
  darkGreen: "text-[#064e3b]"
};

const apiKey = ""; // API Key provided by environment

const App = () => {
  const [isScrolled, setIsScrolled] = useState(false);
  const [mobileMenuOpen, setMobileMenuOpen] = useState(false);

  // --- AI Tool State ---
  const [activeAiTool, setActiveAiTool] = useState('hooks'); // 'hooks' or 'strategy'
  const [aiInput, setAiInput] = useState('');
  const [aiResponse, setAiResponse] = useState(null);
  const [isGenerating, setIsGenerating] = useState(false);
  const [aiError, setAiError] = useState(null);

  // Handle scroll for navbar styling
  useEffect(() => {
    const handleScroll = () => {
      setIsScrolled(window.scrollY > 50);
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  const scrollToSection = (id) => {
    const element = document.getElementById(id);
    if (element) {
      element.scrollIntoView({ behavior: 'smooth' });
      setMobileMenuOpen(false);
    }
  };

  // --- AI Generation Logic ---
  const handleGenerate = async (e) => {
    e.preventDefault();
    if (!aiInput.trim()) return;

    setIsGenerating(true);
    setAiError(null);
    setAiResponse(null);

    const prompt = activeAiTool === 'hooks' 
      ? `Act as a viral content strategist for Outbox Media. Generate 3 high-retention, punchy video hooks and 1 short video concept for the topic: "${aiInput}". Format the output clearly with emojis. Keep it brief and punchy.`
      : `Act as a business growth consultant for Outbox Media. Suggest 3 specific short-form video ideas for a "${aiInput}" business to get more customers. Focus on visual storytelling and ROI. Keep it brief.`;

    try {
      const response = await fetch(
        `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`,
        {
          method: 'POST',
          headers: {
            'Content-Type': 'application/json',
          },
          body: JSON.stringify({
            contents: [{ parts: [{ text: prompt }] }],
          }),
        }
      );

      if (!response.ok) {
        throw new Error('Failed to generate content');
      }

      const data = await response.json();
      const text = data.candidates?.[0]?.content?.parts?.[0]?.text;
      setAiResponse(text);
    } catch (error) {
      setAiError("Something went wrong. Please try again.");
      console.error(error);
    } finally {
      setIsGenerating(false);
    }
  };

  return (
    <div className={`min-h-screen ${brandColors.bg} font-sans text-slate-900 selection:bg-yellow-200`}>
      
      {/* --- Navigation --- */}
      <nav className={`fixed w-full z-50 transition-all duration-300 ${isScrolled ? 'bg-white/90 backdrop-blur-md shadow-sm py-4' : 'bg-transparent py-6'}`}>
        <div className="container mx-auto px-6 flex justify-between items-center">
          {/* Logo Representation */}
          <div className="flex items-center space-x-2 cursor-pointer" onClick={() => window.scrollTo(0,0)}>
            <div className="relative font-bold text-2xl tracking-tighter flex items-center">
              <span className={brandColors.teal}>OUT</span>
              <span className={brandColors.blue}>BOX</span>
              <span className={`ml-2 ${brandColors.dark} font-medium tracking-widest text-sm border-l-2 border-black pl-2`}>MEDIA</span>
            </div>
          </div>

          {/* Desktop Links */}
          <div className="hidden md:flex items-center space-x-8 font-medium text-sm uppercase tracking-wider text-gray-600">
            <button onClick={() => scrollToSection('approach')} className="hover:text-[#0056b3] transition-colors">Approach</button>
            <button onClick={() => scrollToSection('services')} className="hover:text-[#0056b3] transition-colors">Packages</button>
            <button onClick={() => scrollToSection('ai-tools')} className="hover:text-[#0056b3] transition-colors flex items-center gap-1"><Sparkles size={14} className="text-purple-600" /> AI Tools</button>
            <button onClick={() => scrollToSection('process')} className="hover:text-[#0056b3] transition-colors">Process</button>
            <button 
              onClick={() => scrollToSection('contact')}
              className={`${brandColors.tealBg} text-white px-6 py-2.5 rounded-full hover:opacity-90 transition-all shadow-lg shadow-teal-900/20`}
            >
              Start Growth
            </button>
          </div>

          {/* Mobile Menu Toggle */}
          <button className="md:hidden" onClick={() => setMobileMenuOpen(!mobileMenuOpen)}>
            {mobileMenuOpen ? <X size={28} /> : <Menu size={28} />}
          </button>
        </div>

        {/* Mobile Menu */}
        {mobileMenuOpen && (
          <div className="absolute top-full left-0 w-full bg-white border-b border-gray-100 p-6 md:hidden flex flex-col space-y-4 shadow-xl">
            <button onClick={() => scrollToSection('approach')} className="text-left py-2 font-medium text-gray-700">Approach</button>
            <button onClick={() => scrollToSection('services')} className="text-left py-2 font-medium text-gray-700">Packages</button>
            <button onClick={() => scrollToSection('ai-tools')} className="text-left py-2 font-medium text-gray-700">AI Tools</button>
            <button onClick={() => scrollToSection('process')} className="text-left py-2 font-medium text-gray-700">Process</button>
            <button onClick={() => scrollToSection('contact')} className={`${brandColors.tealBg} text-white py-3 rounded-lg text-center`}>Start Growth</button>
          </div>
        )}
      </nav>

      {/* --- Hero Section --- */}
      <header className="relative pt-32 pb-20 lg:pt-48 lg:pb-32 overflow-hidden">
        <div className="container mx-auto px-6 relative z-10">
          <div className="max-w-4xl">
            <div className="inline-flex items-center space-x-2 bg-white border border-gray-200 rounded-full px-4 py-1.5 mb-8 shadow-sm animate-fade-in-up">
              <span className={`w-2 h-2 rounded-full ${brandColors.yellowBg}`}></span>
              <span className="text-xs font-bold uppercase tracking-wider text-gray-500">For Business Owners & Brands</span>
            </div>
            
            <h1 className="text-5xl md:text-7xl font-bold leading-[1.1] mb-8 text-[#1a1a1a]">
              We Build <span className="relative inline-block">
                <span className={`relative z-10 ${brandColors.blue}`}>Content Engines</span>
                <svg className="absolute bottom-2 left-0 w-full h-3 text-yellow-300 -z-10" viewBox="0 0 100 10" preserveAspectRatio="none">
                  <path d="M0 5 Q 50 10 100 5" stroke="currentColor" strokeWidth="8" fill="none" />
                </svg>
              </span> <br />
              That Grow Businesses.
            </h1>
            
            <p className="text-xl md:text-2xl text-gray-600 max-w-2xl mb-10 leading-relaxed">
              Stop chasing viral flukes. Get a complete content solution designed for founders—from ideation to retention-focused editing and revenue growth.
            </p>
            
            <div className="flex flex-col sm:flex-row gap-4">
              <button onClick={() => scrollToSection('services')} className={`${brandColors.blueBg} text-white px-8 py-4 rounded-full font-bold text-lg hover:translate-y-[-2px] transition-all shadow-xl shadow-blue-900/20 flex items-center justify-center gap-2`}>
                View Packages <ArrowRight size={20} />
              </button>
              <button onClick={() => scrollToSection('contact')} className="bg-white border-2 border-gray-200 text-gray-800 px-8 py-4 rounded-full font-bold text-lg hover:border-gray-400 transition-all flex items-center justify-center">
                Book Strategy Call
              </button>
            </div>
          </div>
        </div>

        {/* Background Abstract Elements derived from Logo Shapes */}
        <div className="absolute top-0 right-0 w-1/3 h-full opacity-5 pointer-events-none hidden lg:block">
           {/* Abstract geometric shapes representing the logo */}
           <div className={`absolute top-20 right-20 w-64 h-64 rounded-full ${brandColors.tealBg} blur-3xl`}></div>
           <div className={`absolute top-60 right-60 w-40 h-40 rounded-full ${brandColors.yellowBg} blur-2xl`}></div>
        </div>
      </header>

      {/* --- Marquee / Trust Bar --- */}
      <div className="bg-black py-6 overflow-hidden whitespace-nowrap">
        <div className="inline-flex items-center animate-marquee">
          {[...Array(2)].map((_, i) => (
            <div key={i} className="flex items-center">
              <span className="text-white/50 text-xl font-bold mx-8 uppercase tracking-widest">Retention</span>
              <span className="text-yellow-500 text-xl mx-4">•</span>
              <span className="text-white/50 text-xl font-bold mx-8 uppercase tracking-widest">Strategy</span>
              <span className="text-yellow-500 text-xl mx-4">•</span>
              <span className="text-white/50 text-xl font-bold mx-8 uppercase tracking-widest">Growth</span>
              <span className="text-yellow-500 text-xl mx-4">•</span>
              <span className="text-white/50 text-xl font-bold mx-8 uppercase tracking-widest">Scripting</span>
              <span className="text-yellow-500 text-xl mx-4">•</span>
              <span className="text-white/50 text-xl font-bold mx-8 uppercase tracking-widest">Automation</span>
              <span className="text-yellow-500 text-xl mx-4">•</span>
            </div>
          ))}
        </div>
      </div>

      {/* --- The Problem vs Solution (Approach) --- */}
      <section id="approach" className="py-24 bg-white">
        <div className="container mx-auto px-6">
          <div className="text-center max-w-3xl mx-auto mb-16">
            <h2 className="text-sm font-bold uppercase tracking-widest text-gray-500 mb-3">The Reality</h2>
            <h3 className="text-3xl md:text-4xl font-bold text-gray-900">Why Most Business Content Fails</h3>
          </div>

          <div className="grid md:grid-cols-3 gap-12">
            {/* Card 1 */}
            <div className="bg-gray-50 p-8 rounded-2xl border border-gray-100 hover:shadow-lg transition-shadow">
              <div className="w-12 h-12 bg-red-100 rounded-xl flex items-center justify-center text-red-600 mb-6">
                <Video size={24} />
              </div>
              <h4 className="text-xl font-bold mb-3">Random Editing</h4>
              <p className="text-gray-600 leading-relaxed">Pretty cuts and flashy transitions that look cool but don't tell a story or convert viewers into customers.</p>
            </div>

            {/* Card 2 */}
            <div className="bg-gray-50 p-8 rounded-2xl border border-gray-100 hover:shadow-lg transition-shadow">
              <div className="w-12 h-12 bg-orange-100 rounded-xl flex items-center justify-center text-orange-600 mb-6">
                <TrendingUp size={24} />
              </div>
              <h4 className="text-xl font-bold mb-3">Influencer Tactics</h4>
              <p className="text-gray-600 leading-relaxed">Chasing childish trends that damage your brand's authority instead of building trust with serious clients.</p>
            </div>

            {/* Card 3 (The Solution) */}
            <div className={`${brandColors.tealBg} p-8 rounded-2xl text-white shadow-xl transform md:-translate-y-4`}>
              <div className="w-12 h-12 bg-white/20 rounded-xl flex items-center justify-center text-white mb-6">
                <CheckCircle size={24} />
              </div>
              <h4 className="text-xl font-bold mb-3">The Outbox Way</h4>
              <p className="text-teal-100 leading-relaxed">We engineer retention. We combine scripting, pacing, and psychology to turn viewers into leads. Business-first content.</p>
            </div>
          </div>
        </div>
      </section>

      {/* --- Services / Packages --- */}
      <section id="services" className={`py-24 ${brandColors.bg}`}>
        <div className="container mx-auto px-6">
          <div className="mb-16">
            <h2 className="text-4xl md:text-5xl font-bold mb-6 text-gray-900">Complete Content Solutions</h2>
            <p className="text-xl text-gray-600 max-w-2xl">Choose the engine that fits your business stage. From editing to full automation.</p>
          </div>

          <div className="grid lg:grid-cols-3 gap-8">
            
            {/* Package 1 - Teal Accent */}
            <div className="bg-white rounded-3xl p-8 border-2 border-transparent hover:border-teal-600/20 shadow-xl shadow-gray-200/50 transition-all group relative overflow-hidden flex flex-col">
              <div className={`absolute top-0 left-0 w-full h-2 ${brandColors.tealBg}`}></div>
              <div className="mb-8">
                <span className={`inline-block px-3 py-1 rounded-full bg-teal-50 ${brandColors.teal} text-xs font-bold uppercase tracking-wider mb-4`}>
                  Package 01
                </span>
                <h3 className="text-2xl font-bold mb-2">High-Retention Editing</h3>
                <p className="text-gray-500 text-sm">For brands who shoot their own footage.</p>
              </div>
              
              <ul className="space-y-4 mb-8 flex-grow">
                {[
                  "20–22 Edited Videos/Month",
                  "High-Retention Style",
                  "AI B-Rolls & Graphics",
                  "Captions & Sound Design",
                  "Trend Research Included"
                ].map((item, i) => (
                  <li key={i} className="flex items-start">
                    <CheckCircle size={18} className={`mr-3 mt-1 ${brandColors.teal} flex-shrink-0`} />
                    <span className="text-gray-700 text-sm font-medium">{item}</span>
                  </li>
                ))}
              </ul>

              <div className="mt-auto">
                 <p className="text-xs text-gray-500 mb-4 border-t pt-4">Outcome: Higher Reach & Better Retention.</p>
                <button className={`w-full py-3 rounded-xl border-2 border-teal-600 ${brandColors.teal} font-bold hover:bg-teal-600 hover:text-white transition-colors`}>
                  Select Package
                </button>
              </div>
            </div>

            {/* Package 2 - Blue Accent (Popular) */}
            <div className="bg-[#0b1120] rounded-3xl p-8 border-2 border-blue-500 shadow-2xl relative overflow-hidden transform lg:-translate-y-4 flex flex-col">
              <div className="absolute top-0 right-0 bg-blue-600 text-white text-xs font-bold px-4 py-1 rounded-bl-xl">MOST POPULAR</div>
              
              <div className="mb-8">
                <span className="inline-block px-3 py-1 rounded-full bg-blue-900/50 text-blue-400 text-xs font-bold uppercase tracking-wider mb-4">
                  Package 02
                </span>
                <h3 className="text-2xl font-bold mb-2 text-white">Content Growth + Mgmt</h3>
                <p className="text-gray-400 text-sm">Complete "Done-For-You" Management.</p>
              </div>
              
              <ul className="space-y-4 mb-8 flex-grow">
                <li className="text-blue-400 font-semibold text-sm flex items-center">
                   <span className="w-1.5 h-1.5 rounded-full bg-blue-400 mr-2"></span>
                   Everything in Package 1 PLUS:
                </li>
                {[
                  "Full Social Media Mgmt",
                  "Uploading & Scheduling",
                  "Hashtags & SEO",
                  "Caption Copywriting",
                  "Monthly Strategy Calls",
                  "Performance Reports"
                ].map((item, i) => (
                  <li key={i} className="flex items-start">
                    <CheckCircle size={18} className="mr-3 mt-1 text-blue-500 flex-shrink-0" />
                    <span className="text-gray-300 text-sm font-medium">{item}</span>
                  </li>
                ))}
              </ul>

              <div className="mt-auto">
                <p className="text-xs text-gray-500 mb-4 border-t border-gray-800 pt-4">Outcome: Consistent Growth, Zero Stress.</p>
                <button className={`w-full py-3 rounded-xl ${brandColors.blueBg} text-white font-bold hover:bg-blue-500 transition-colors shadow-lg shadow-blue-900/50`}>
                  Start Growth
                </button>
              </div>
            </div>

            {/* Package 3 - Purple Accent */}
            <div className="bg-white rounded-3xl p-8 border-2 border-transparent hover:border-indigo-600/20 shadow-xl shadow-gray-200/50 transition-all flex flex-col">
               <div className={`absolute top-0 left-0 w-full h-2 ${brandColors.purpleBg}`}></div>
              <div className="mb-8">
                <span className={`inline-block px-3 py-1 rounded-full bg-indigo-50 ${brandColors.purple} text-xs font-bold uppercase tracking-wider mb-4`}>
                  Package 03
                </span>
                <h3 className="text-2xl font-bold mb-2">AI-Avatar Automation</h3>
                <p className="text-gray-500 text-sm">For founders who hate being on camera.</p>
              </div>
              
              <ul className="space-y-4 mb-8 flex-grow">
                 <li className={`${brandColors.purple} font-semibold text-sm flex items-center`}>
                   <span className={`w-1.5 h-1.5 rounded-full ${brandColors.purpleBg} mr-2`}></span>
                   Everything in Package 2 PLUS:
                </li>
                {[
                  "Real 3D/Realistic AI Avatars",
                  "Zero Shooting Required",
                  "Voice Cloning & Automation",
                  "Full Production (Script to Post)",
                  "5 Hours/Month Founder Time"
                ].map((item, i) => (
                  <li key={i} className="flex items-start">
                    <CheckCircle size={18} className={`mr-3 mt-1 ${brandColors.purple} flex-shrink-0`} />
                    <span className="text-gray-700 text-sm font-medium">{item}</span>
                  </li>
                ))}
              </ul>

              <div className="mt-auto">
                <p className="text-xs text-gray-500 mb-4 border-t pt-4">Outcome: A Personal Brand on Autopilot.</p>
                <button className={`w-full py-3 rounded-xl border-2 border-indigo-600 ${brandColors.purple} font-bold hover:bg-indigo-600 hover:text-white transition-colors`}>
                  Learn More
                </button>
              </div>
            </div>

          </div>
        </div>
      </section>

      {/* --- AI TOOLS SECTION (NEW) --- */}
      <section id="ai-tools" className="py-24 bg-[#111] text-white relative overflow-hidden">
        <div className="absolute top-0 right-0 w-1/2 h-full bg-gradient-to-l from-indigo-900/20 to-transparent pointer-events-none"></div>
        
        <div className="container mx-auto px-6 relative z-10">
          <div className="flex flex-col lg:flex-row gap-12 items-start">
            {/* Left Side: Intro */}
            <div className="lg:w-1/3">
              <div className="inline-flex items-center space-x-2 bg-white/10 border border-white/10 rounded-full px-4 py-1.5 mb-6">
                <Sparkles size={14} className="text-yellow-400" />
                <span className="text-xs font-bold uppercase tracking-wider text-white/80">Powered by Gemini AI</span>
              </div>
              <h2 className="text-4xl font-bold mb-6">Experience Our Content Engine</h2>
              <p className="text-gray-400 mb-8 leading-relaxed">
                See how our systems work. Try our internal AI tools to generate viral hooks or content strategies instantly.
              </p>
              
              <div className="flex flex-col gap-3">
                <button 
                  onClick={() => { setActiveAiTool('hooks'); setAiResponse(null); setAiInput(''); }}
                  className={`px-6 py-4 rounded-xl text-left transition-all border ${activeAiTool === 'hooks' ? 'bg-indigo-600 border-indigo-500 text-white' : 'bg-white/5 border-white/10 text-gray-400 hover:bg-white/10'}`}
                >
                  <div className="flex items-center justify-between mb-1">
                    <span className="font-bold flex items-center gap-2"><Zap size={18} /> ✨ Viral Hook Generator</span>
                    {activeAiTool === 'hooks' && <div className="w-2 h-2 bg-white rounded-full animate-pulse"></div>}
                  </div>
                  <p className="text-xs opacity-70">Generate 3 high-retention hooks for any topic.</p>
                </button>

                <button 
                  onClick={() => { setActiveAiTool('strategy'); setAiResponse(null); setAiInput(''); }}
                  className={`px-6 py-4 rounded-xl text-left transition-all border ${activeAiTool === 'strategy' ? 'bg-indigo-600 border-indigo-500 text-white' : 'bg-white/5 border-white/10 text-gray-400 hover:bg-white/10'}`}
                >
                  <div className="flex items-center justify-between mb-1">
                    <span className="font-bold flex items-center gap-2"><BarChart3 size={18} /> ✨ Growth Strategy Planner</span>
                    {activeAiTool === 'strategy' && <div className="w-2 h-2 bg-white rounded-full animate-pulse"></div>}
                  </div>
                  <p className="text-xs opacity-70">Get a mini content calendar for your niche.</p>
                </button>
              </div>
            </div>

            {/* Right Side: Interactive Tool */}
            <div className="lg:w-2/3 w-full">
              <div className="bg-[#1a1a1a] border border-white/10 rounded-2xl p-8 h-full min-h-[400px] flex flex-col shadow-2xl">
                
                <form onSubmit={handleGenerate} className="mb-6">
                  <label className="block text-sm font-medium text-gray-400 mb-2">
                    {activeAiTool === 'hooks' ? 'Enter a Video Topic (e.g., "Real Estate Tips")' : 'Enter Your Business Type (e.g., "Coffee Shop")'}
                  </label>
                  <div className="flex gap-3">
                    <input 
                      type="text" 
                      value={aiInput}
                      onChange={(e) => setAiInput(e.target.value)}
                      placeholder={activeAiTool === 'hooks' ? 'e.g. How to buy a house' : 'e.g. Personal Trainer'}
                      className="flex-1 bg-black/50 border border-white/20 rounded-xl px-5 py-4 text-white placeholder-gray-600 focus:outline-none focus:border-indigo-500 transition-colors"
                    />
                    <button 
                      type="submit" 
                      disabled={isGenerating || !aiInput}
                      className="bg-indigo-600 hover:bg-indigo-500 disabled:opacity-50 disabled:cursor-not-allowed text-white px-8 py-4 rounded-xl font-bold transition-colors flex items-center gap-2"
                    >
                      {isGenerating ? <Loader2 size={20} className="animate-spin" /> : <Sparkles size={20} />}
                      Generate
                    </button>
                  </div>
                </form>

                <div className="flex-grow bg-black/30 rounded-xl border border-white/5 p-6 font-mono text-sm overflow-auto">
                  {isGenerating ? (
                    <div className="flex flex-col items-center justify-center h-full text-gray-500 gap-3">
                      <Loader2 size={32} className="animate-spin text-indigo-500" />
                      <p>Consulting the AI Engine...</p>
                    </div>
                  ) : aiResponse ? (
                    <div className="whitespace-pre-wrap leading-relaxed text-gray-200">
                      {aiResponse}
                    </div>
                  ) : aiError ? (
                    <div className="flex flex-col items-center justify-center h-full text-red-400">
                       <p>{aiError}</p>
                    </div>
                  ) : (
                    <div className="flex flex-col items-center justify-center h-full text-gray-600">
                      <Cpu size={48} className="mb-4 opacity-20" />
                      <p className="text-center">Ready to generate.<br/>Select a tool and enter a prompt.</p>
                    </div>
                  )}
                </div>
                
                <div className="mt-4 text-xs text-gray-600 flex justify-between items-center">
                   <span>Results generated by Gemini 1.5 Flash</span>
                   <span className="text-indigo-400">Outbox Media Internal Tools v1.0</span>
                </div>

              </div>
            </div>
          </div>
        </div>
      </section>

      {/* --- Process Section --- */}
      <section id="process" className="py-24 bg-white relative overflow-hidden">
        {/* Decorative Background line */}
        <div className="absolute top-1/2 left-0 w-full h-px bg-gray-100 -z-10 hidden md:block"></div>

        <div className="container mx-auto px-6">
          <div className="text-center mb-20">
            <h2 className="text-4xl font-bold mb-4">Your Content, Systematized</h2>
            <p className="text-gray-500">From raw idea to revenue-generating asset.</p>
          </div>

          <div className="grid md:grid-cols-4 gap-8">
            {[
              { icon: <Users />, title: "Strategy", desc: "We research trends and write scripts that hook your ideal client." },
              { icon: <Video />, title: "Production", desc: "Whether you shoot or we use AI, we edit for maximum watch time." },
              { icon: <BarChart3 />, title: "Growth", desc: "We manage the upload and track analytics to scale results." },
              { icon: <TrendingUp />, title: "Scale", desc: "Consistent output leads to compounding brand authority." },
            ].map((step, idx) => (
              <div key={idx} className="relative bg-white p-6 rounded-xl border border-gray-100 shadow-sm group hover:-translate-y-2 transition-transform">
                <div className={`w-14 h-14 rounded-full ${brandColors.bg} flex items-center justify-center ${brandColors.blue} mb-6 group-hover:scale-110 transition-transform`}>
                  {step.icon}
                </div>
                <h4 className="text-xl font-bold mb-2">{step.title}</h4>
                <p className="text-sm text-gray-600 leading-relaxed">{step.desc}</p>
                {idx < 3 && (
                  <div className="hidden md:block absolute top-1/2 -right-4 transform -translate-y-1/2 text-gray-300">
                    <ChevronRight size={24} />
                  </div>
                )}
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* --- Contact Section --- */}
      <section id="contact" className={`${brandColors.blueBg} py-24 text-white`}>
        <div className="container mx-auto px-6">
          <div className="grid md:grid-cols-2 gap-16 items-center">
            <div>
              <h2 className="text-4xl md:text-5xl font-bold mb-6">Ready to Outbox the Competition?</h2>
              <p className="text-blue-100 text-lg mb-8">
                Let's build a content engine that works as hard as you do. Book a free strategy call to see which package fits your business.
              </p>
              
              <div className="space-y-6">
                <div className="flex items-center space-x-4">
                  <div className="w-12 h-12 bg-white/10 rounded-full flex items-center justify-center">
                    <Mail className="text-yellow-400" />
                  </div>
                  <div>
                    <p className="text-sm text-blue-200 uppercase tracking-wider">Email Us</p>
                    <p className="font-medium">hello@outboxmedia.com</p>
                  </div>
                </div>
                 <div className="flex items-center space-x-4">
                  <div className="w-12 h-12 bg-white/10 rounded-full flex items-center justify-center">
                    <Users className="text-yellow-400" />
                  </div>
                  <div>
                    <p className="text-sm text-blue-200 uppercase tracking-wider">Follow Us</p>
                    <div className="flex space-x-4 mt-1">
                      <a href="#" className="hover:text-yellow-400 transition-colors"><Instagram size={20} /></a>
                      <a href="#" className="hover:text-yellow-400 transition-colors"><Linkedin size={20} /></a>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div className="bg-white text-gray-900 p-8 rounded-3xl shadow-2xl">
              <form className="space-y-4">
                <div>
                  <label className="block text-sm font-bold text-gray-700 mb-1">Full Name</label>
                  <input type="text" className="w-full px-4 py-3 rounded-lg bg-gray-50 border border-gray-200 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all" placeholder="John Doe" />
                </div>
                <div>
                  <label className="block text-sm font-bold text-gray-700 mb-1">Business Name</label>
                  <input type="text" className="w-full px-4 py-3 rounded-lg bg-gray-50 border border-gray-200 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all" placeholder="Company Ltd." />
                </div>
                <div>
                  <label className="block text-sm font-bold text-gray-700 mb-1">Interested In</label>
                  <select className="w-full px-4 py-3 rounded-lg bg-gray-50 border border-gray-200 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all">
                    <option>High-Retention Editing (Pkg 1)</option>
                    <option>Growth + Management (Pkg 2)</option>
                    <option>AI-Avatar Automation (Pkg 3)</option>
                    <option>Not sure yet</option>
                  </select>
                </div>
                <button className={`w-full py-4 rounded-xl ${brandColors.tealBg} text-white font-bold text-lg hover:opacity-90 transition-opacity mt-4`}>
                  Get Your Free Strategy
                </button>
              </form>
            </div>
          </div>
        </div>
      </section>

      {/* --- Footer --- */}
      <footer className="bg-[#111] text-gray-400 py-12 border-t border-gray-800">
        <div className="container mx-auto px-6 flex flex-col md:flex-row justify-between items-center">
          <div className="flex items-center space-x-2 mb-4 md:mb-0">
             <div className="font-bold text-xl tracking-tighter">
              <span className="text-teal-600">OUT</span>
              <span className="text-blue-600">BOX</span>
              <span className="ml-2 text-white font-medium tracking-widest text-sm border-l-2 border-gray-600 pl-2">MEDIA</span>
            </div>
          </div>
          <div className="text-sm">
            &copy; {new Date().getFullYear()} Outbox Media. All rights reserved.
          </div>
        </div>
      </footer>

    </div>
  );
};

export default App;