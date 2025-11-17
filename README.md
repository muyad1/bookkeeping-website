# bookkeeping-website
This is my first bookkeeping website created from ChatGPT

import React from "react";

// MUYAD Bookkeeping - Single-file React component (TailwindCSS)
// Usage: drop into a Create React App / Next.js page with Tailwind set up.
// Fonts used: Montserrat (headings) + Inter (body). Include them in your index.html

export default function MuyadHomepage() {
  return (
    <div className="min-h-screen bg-gray-50 text-slate-800 font-inter">
      {/* Header */}
      <header className="bg-white border-b border-gray-200">
        <div className="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
          <div className="flex items-center gap-3">
            <div className="w-12 h-12 rounded-md flex items-center justify-center bg-[#0A2342] text-white">
              <span className="font-bold text-lg">M</span>
            </div>
            <div>
              <h1 className="text-xl font-semibold text-[#0A2342]">MUYAD Bookkeeping</h1>
              <p className="text-sm text-slate-500 -mt-1">Your numbers, made simple.</p>
            </div>
          </div>

          <nav className="hidden md:flex items-center gap-6 text-sm">
            <a href="#services" className="hover:text-[#0FB5B0]">Services</a>
            <a href="#how" className="hover:text-[#0FB5B0]">How it works</a>
            <a href="#pricing" className="hover:text-[#0FB5B0]">Pricing</a>
            <a href="#contact" className="px-4 py-2 bg-[#0FB5B0] text-white rounded-md">Get Started</a>
          </nav>

          <div className="md:hidden">
            <button aria-label="menu" className="px-3 py-2 bg-[#0FB5B0] text-white rounded-md">Menu</button>
          </div>
        </div>
      </header>

      {/* Hero */}
      <section className="bg-white">
        <div className="max-w-6xl mx-auto px-6 py-16 grid grid-cols-1 md:grid-cols-2 gap-10 items-center">
          <div>
            <h2 className="text-4xl font-extrabold text-[#0A2342] leading-tight">Professional bookkeeping that grows with your business</h2>
            <p className="mt-4 text-lg text-slate-600">We provide accurate monthly bookkeeping, bank reconciliation, and financial reports so you can focus on running your business with confidence.</p>

            <div className="mt-8 flex gap-4">
              <a href="#contact" className="inline-block px-6 py-3 bg-[#0FB5B0] text-white rounded-md font-medium">Start with a free audit</a>
              <a href="#services" className="inline-block px-6 py-3 border border-[#0A2342] text-[#0A2342] rounded-md font-medium">View services</a>
            </div>

            <div className="mt-8 flex items-center gap-6 text-sm text-slate-500">
              <div className="flex items-center gap-3">
                <div className="w-10 h-10 rounded-full flex items-center justify-center bg-[#E6E8EB]">📊</div>
                <div>
                  <div className="font-semibold text-slate-800">Monthly reports</div>
                  <div className="text-xs">P&L, Balance Sheet, Cash flow</div>
                </div>
              </div>

              <div className="flex items-center gap-3">
                <div className="w-10 h-10 rounded-full flex items-center justify-center bg-[#E6E8EB]">✅</div>
                <div>
                  <div className="font-semibold text-slate-800">QuickBooks Certified</div>
                  <div className="text-xs">Reliable bookkeeping workflows</div>
                </div>
              </div>
            </div>
          </div>

          <div className="bg-[#F8FAFB] p-8 rounded-lg shadow-sm">
            <div className="bg-white rounded-md p-6 border border-gray-100">
              <h3 className="text-lg font-semibold text-[#0A2342]">Free bookkeeping audit</h3>
              <p className="mt-2 text-sm text-slate-600">Send us your records and we'll review your books, point out quick wins and errors, and show you how to save time.</p>

              <form className="mt-4 space-y-3">
                <input className="w-full border border-gray-200 rounded-md px-3 py-2 text-sm" placeholder="Your name" />
                <input className="w-full border border-gray-200 rounded-md px-3 py-2 text-sm" placeholder="Business name" />
                <input className="w-full border border-gray-200 rounded-md px-3 py-2 text-sm" placeholder="Email or WhatsApp" />
                <button className="w-full mt-2 px-4 py-2 bg-[#0A2342] text-white rounded-md">Request audit</button>
              </form>
            </div>
          </div>
        </div>
      </section>

      {/* Services */}
      <section id="services" className="max-w-6xl mx-auto px-6 py-12">
        <h3 className="text-2xl font-semibold text-[#0A2342]">Services</h3>
        <p className="mt-2 text-slate-600">Tailored bookkeeping packages for small and growing businesses.</p>

        <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <h4 className="font-semibold text-lg">Monthly Bookkeeping</h4>
            <p className="mt-2 text-sm text-slate-600">Complete bookkeeping and reporting for small businesses.</p>
            <div className="mt-4 text-sm font-medium text-[#0A2342]">From ₦25,000/month</div>
          </div>

          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <h4 className="font-semibold text-lg">Bank Reconciliation</h4>
            <p className="mt-2 text-sm text-slate-600">We match every transaction and fix discrepancies.</p>
            <div className="mt-4 text-sm font-medium text-[#0A2342]">Fixed fee</div>
          </div>

          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <h4 className="font-semibold text-lg">Invoicing & Collections</h4>
            <p className="mt-2 text-sm text-slate-600">Send invoices and keep track of payments efficiently.</p>
            <div className="mt-4 text-sm font-medium text-[#0A2342]">Add-on service</div>
          </div>
        </div>
      </section>

      {/* How it works */}
      <section id="how" className="bg-white border-t border-b border-gray-100">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h3 className="text-2xl font-semibold text-[#0A2342]">How it works</h3>
          <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
            <div className="p-6 bg-[#F8FAFB] rounded-lg">
              <div className="font-semibold">1. Send your records</div>
              <div className="text-sm text-slate-600 mt-2">Bank statements, receipts, sales reports.</div>
            </div>
            <div className="p-6 bg-[#F8FAFB] rounded-lg">
              <div className="font-semibold">2. We clean & categorise</div>
              <div className="text-sm text-slate-600 mt-2">Data entry, reconciliations, classification.</div>
            </div>
            <div className="p-6 bg-[#F8FAFB] rounded-lg">
              <div className="font-semibold">3. Monthly reports</div>
              <div className="text-sm text-slate-600 mt-2">P&L, Balance Sheet, cashflow + recommendations.</div>
            </div>
          </div>
        </div>
      </section>

      {/* Testimonials */}
      <section className="max-w-6xl mx-auto px-6 py-12">
        <h3 className="text-2xl font-semibold text-[#0A2342]">Trusted by business owners</h3>
        <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <p className="text-slate-600">"Muyad made our accounts accurate and painless. Highly recommended."</p>
            <div className="mt-4 font-semibold text-sm">— Aisha, Salon Owner</div>
          </div>

          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <p className="text-slate-600">"Fast, reliable, and always on time with reports."</p>
            <div className="mt-4 font-semibold text-sm">— Chinedu, E‑commerce Seller</div>
          </div>

          <div className="p-6 bg-white rounded-lg border border-gray-100">
            <p className="text-slate-600">"Professional service — our books are finally organised."</p>
            <div className="mt-4 font-semibold text-sm">— Funmi, Food Business</div>
          </div>
        </div>
      </section>

      {/* Contact / CTA */}
      <section id="contact" className="bg-[#0A2342] text-white">
        <div className="max-w-6xl mx-auto px-6 py-12 grid grid-cols-1 md:grid-cols-2 gap-6 items-center">
          <div>
            <h3 className="text-2xl font-semibold">Ready to get your books in order?</h3>
            <p className="mt-2 text-slate-200">Request a free audit and we will show you where to save time and improve cashflow.</p>
          </div>

          <div>
            <form className="space-y-3">
              <input placeholder="Your name" className="w-full px-3 py-2 rounded-md text-slate-800" />
              <input placeholder="Business name" className="w-full px-3 py-2 rounded-md text-slate-800" />
              <input placeholder="Email or WhatsApp" className="w-full px-3 py-2 rounded-md text-slate-800" />
              <button className="w-full px-4 py-2 bg-[#0FB5B0] text-[#0A2342] font-semibold rounded-md">Request free audit</button>
            </form>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-white border-t border-gray-100">
        <div className="max-w-6xl mx-auto px-6 py-8 flex flex-col md:flex-row items-center justify-between gap-4">
          <div className="text-sm text-slate-600">© {new Date().getFullYear()} MUYAD Bookkeeping. All rights reserved.</div>
          <div className="flex items-center gap-4 text-sm">
            <a className="hover:text-[#0FB5B0]">Privacy</a>
            <a className="hover:text-[#0FB5B0]">Terms</a>
            <a className="hover:text-[#0FB5B0]">Contact</a>
          </div>
        </div>
      </footer>
    </div>
  );
}
