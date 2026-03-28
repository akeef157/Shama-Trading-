import React from "react";
import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";
import { Phone, MessageCircle, Ship, PlayCircle, Car, Bike, ShieldCheck, ChevronRight, Globe2, Star } from "lucide-react";

const cars = [
  {
    name: "Honda NSX",
    tag: "Sports Icon",
    desc: "Legendary Japanese performance styling with an unforgettable road presence.",
    image:
      "https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=1200&q=80",
  },
  {
    name: "Toyota Crown",
    tag: "Luxury Sedan",
    desc: "Premium comfort, clean lines, and a refined executive feel from Japan.",
    image:
      "https://images.unsplash.com/photo-1494976388531-d1058494cdd8?auto=format&fit=crop&w=1200&q=80",
  },
  {
    name: "Nissan GT-R",
    tag: "Performance Beast",
    desc: "A bold high-power machine built for speed lovers and prestige buyers.",
    image:
      "https://images.unsplash.com/photo-1544636331-e26879cd4d9b?auto=format&fit=crop&w=1200&q=80",
  },
];

const bikes = [
  {
    name: "Honda PCX",
    tag: "Urban Favorite",
    desc: "Stylish, reliable, and perfect for city commuting with premium comfort.",
    image:
      "https://images.unsplash.com/photo-1558981806-ec527fa84c39?auto=format&fit=crop&w=1200&q=80",
  },
  {
    name: "Yamaha NMAX",
    tag: "Modern Scooter",
    desc: "Smooth ride quality, efficient design, and practical everyday performance.",
    image:
      "https://images.unsplash.com/photo-1517846693594-1567da72af75?auto=format&fit=crop&w=1200&q=80",
  },
  {
    name: "Kawasaki Ninja",
    tag: "Sport Bike",
    desc: "Sharp lines, energetic character, and a thrilling premium bike image.",
    image:
      "https://images.unsplash.com/photo-1609630875171-b1321377ee65?auto=format&fit=crop&w=1200&q=80",
  },
];

const services = [
  {
    icon: Ship,
    title: "Japan Export Support",
    text: "From sourcing to shipping coordination, built for smooth international buying.",
  },
  {
    icon: ShieldCheck,
    title: "Trusted Vehicle Selection",
    text: "Carefully presented cars and motorcycles with premium visual presentation.",
  },
  {
    icon: Globe2,
    title: "Worldwide Inquiry Ready",
    text: "Fast responses through WhatsApp and direct call for overseas customers.",
  },
];

const videos = [
  "Arrival walkarounds",
  "Engine sound previews",
  "Interior detail videos",
  "Bike feature showcases",
];

export default function ShamaTradingNeonMotors() {
  return (
    <div className="min-h-screen bg-[#070b14] text-white">
      <div className="fixed inset-0 -z-10 bg-[radial-gradient(circle_at_top_left,rgba(34,211,238,0.16),transparent_20%),radial-gradient(circle_at_top_right,rgba(249,115,22,0.18),transparent_22%),radial-gradient(circle_at_bottom_left,rgba(217,70,239,0.16),transparent_20%),linear-gradient(180deg,#070b14_0%,#0b1320_55%,#070b14_100%)]" />

      <header className="sticky top-0 z-50 border-b border-white/10 bg-[#070b14]/75 backdrop-blur-xl">
        <div className="mx-auto flex max-w-7xl items-center justify-between px-6 py-4 lg:px-10">
          <div className="flex items-center gap-4">
            <div className="flex h-14 w-14 items-center justify-center rounded-2xl bg-gradient-to-br from-orange-400 via-amber-400 to-cyan-400 text-lg font-black text-slate-950 shadow-2xl shadow-orange-500/20">
              ST
            </div>
            <div>
              <div className="text-2xl font-black tracking-wide">Shama Trading</div>
              <div className="text-sm text-orange-200/80">Used Cars & Motorcycles from Japan</div>
            </div>
          </div>

          <nav className="hidden items-center gap-6 text-sm font-semibold text-white/80 lg:flex">
            <a href="#home" className="hover:text-white">Home</a>
            <a href="#cars" className="hover:text-white">Cars</a>
            <a href="#bikes" className="hover:text-white">Bikes</a>
            <a href="#videos" className="hover:text-white">Videos</a>
            <a href="#contact" className="hover:text-white">Contact</a>
          </nav>
        </div>
      </header>

      <section id="home" className="relative overflow-hidden px-6 pb-20 pt-12 lg:px-10 lg:pt-16">
        <div className="mx-auto grid max-w-7xl gap-10 lg:grid-cols-[1.05fr_0.95fr] lg:items-center">
          <div>
            <Badge className="mb-5 rounded-full border-0 bg-white/10 px-4 py-2 text-white hover:bg-white/10">
              Premium imports from Japan
            </Badge>
            <h1 className="max-w-4xl text-5xl font-black leading-[0.95] md:text-7xl">
              Colorful,
              <span className="block bg-gradient-to-r from-cyan-300 via-fuchsia-400 to-orange-300 bg-clip-text text-transparent">
                bold vehicles
              </span>
              for people who want to stand out.
            </h1>
            <p className="mt-6 max-w-2xl text-lg leading-8 text-white/70 md:text-xl">
              Discover attractive cars and motorcycles from Japan with a premium digital showcase designed to feel modern, beautiful, and unforgettable.
            </p>

            <div className="mt-8 flex flex-wrap gap-3">
              <Button asChild className="rounded-full bg-green-500 px-6 text-white hover:bg-green-400">
                <a href="https://wa.me/818076484545" target="_blank" rel="noreferrer">
                  <MessageCircle className="mr-2 h-4 w-4" />
                  WhatsApp Now
                </a>
              </Button>
              <Button asChild variant="outline" className="rounded-full border-white/20 bg-white/5 px-6 text-white hover:bg-white/10 hover:text-white">
                <a href="tel:+818076484545">
                  <Phone className="mr-2 h-4 w-4" />
                  Call Now
                </a>
              </Button>
              <Button asChild variant="outline" className="rounded-full border-orange-300/30 bg-orange-400/10 px-6 text-orange-100 hover:bg-orange-400/20 hover:text-white">
                <a href="#cars">
                  View Collection
                  <ChevronRight className="ml-2 h-4 w-4" />
                </a>
              </Button>
            </div>

            <div className="mt-10 grid gap-4 sm:grid-cols-3">
              {[
                ["Japan", "Vehicle source"],
                ["Cars + Bikes", "Collection focus"],
                ["Fast", "Direct inquiry"],
              ].map(([big, small]) => (
                <Card key={small} className="rounded-[1.75rem] border-white/10 bg-white/5 backdrop-blur-xl">
                  <CardContent className="p-5">
                    <div className="text-3xl font-black">{big}</div>
                    <div className="mt-1 text-sm text-white/55">{small}</div>
                  </CardContent>
                </Card>
              ))}
            </div>
          </div>

          <motion.div
            initial={{ opacity: 0, y: 24 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.7 }}
            className="relative"
          >
            <div className="absolute -inset-5 rounded-[2rem] bg-gradient-to-r from-cyan-500/20 via-fuchsia-500/20 to-orange-500/20 blur-3xl" />
            <Card className="relative overflow-hidden rounded-[2rem] border border-white/10 bg-white/5 backdrop-blur-2xl">
              <div className="grid gap-0 md:grid-cols-2">
                <div className="min-h-[260px] bg-cover bg-center" style={{ backgroundImage: "url('https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?auto=format&fit=crop&w=1200&q=80')" }} />
                <div className="flex flex-col justify-center p-6">
                  <Badge className="w-fit rounded-full border-0 bg-orange-400/20 text-orange-100 hover:bg-orange-400/20">Featured Style</Badge>
                  <h2 className="mt-4 text-3xl font-black">Premium Cars & Bikes</h2>
                  <p className="mt-3 leading-7 text-white/70">
                    A richer redesign of your original Shama Trading website with stronger visual contrast, more color, cleaner spacing, and a high-end showroom feel.
                  </p>
                  <div className="mt-6 flex items-center gap-3 text-sm text-white/60">
                    <Star className="h-4 w-4 text-yellow-300" /> Beautiful layout
                    <Star className="h-4 w-4 text-cyan-300" /> Attractive design
                  </div>
                </div>
              </div>
            </Card>
          </motion.div>
        </div>
      </section>

      <section id="cars" className="mx-auto max-w-7xl px-6 py-20 lg:px-10">
        <div className="mb-10 flex items-end justify-between gap-4">
          <div>
            <p className="text-sm font-semibold uppercase tracking-[0.3em] text-cyan-300/80">Cars</p>
            <h2 className="mt-3 text-4xl font-black md:text-5xl">Premium car collection</h2>
          </div>
          <a href="https://wa.me/818076484545" target="_blank" rel="noreferrer" className="hidden rounded-full border border-white/15 bg-white/5 px-5 py-3 text-sm font-semibold text-white/85 lg:block">
            Ask on WhatsApp
          </a>
        </div>

        <div className="grid gap-6 md:grid-cols-2 xl:grid-cols-3">
          {cars.map((item, i) => (
            <motion.div
              key={item.name}
              initial={{ opacity: 0, y: 20 }}
              whileInView={{ opacity: 1, y: 0 }}
              viewport={{ once: true, amount: 0.2 }}
              transition={{ duration: 0.5, delay: i * 0.06 }}
            >
              <Card className="group overflow-hidden rounded-[2rem] border-white/10 bg-white/5 transition duration-300 hover:-translate-y-2 hover:bg-white/10 hover:shadow-2xl hover:shadow-cyan-500/10">
                <div className="h-64 bg-cover bg-center transition duration-500 group-hover:scale-105" style={{ backgroundImage: `url('${item.image}')` }} />
                <CardContent className="p-6">
                  <Badge className="rounded-full border-0 bg-cyan-400/15 text-cyan-200 hover:bg-cyan-400/15">{item.tag}</Badge>
                  <h3 className="mt-4 text-2xl font-black">{item.name}</h3>
                  <p className="mt-3 leading-7 text-white/68">{item.desc}</p>
                  <div className="mt-5 text-lg font-bold text-orange-200">Contact for Price</div>
                  <Button asChild className="mt-5 rounded-full bg-white text-slate-950 hover:bg-white/90">
                    <a href="https://wa.me/818076484545" target="_blank" rel="noreferrer">Ask on WhatsApp</a>
                  </Button>
                </CardContent>
              </Card>
            </motion.div>
          ))}
        </div>
      </section>

      <section id="bikes" className="mx-auto max-w-7xl px-6 py-20 lg:px-10">
        <div className="mb-10">
          <p className="text-sm font-semibold uppercase tracking-[0.3em] text-fuchsia-300/80">Bikes</p>
          <h2 className="mt-3 text-4xl font-black md:text-5xl">Modern bike collection</h2>
        </div>

        <div className="grid gap-6 md:grid-cols-2 xl:grid-cols-3">
          {bikes.map((item, i) => (
            <motion.div
              key={item.name}
              initial={{ opacity: 0, y: 20 }}
              whileInView={{ opacity: 1, y: 0 }}
              viewport={{ once: true, amount: 0.2 }}
              transition={{ duration: 0.5, delay: i * 0.06 }}
            >
              <Card className="group overflow-hidden rounded-[2rem] border-white/10 bg-white/5 transition duration-300 hover:-translate-y-2 hover:bg-white/10 hover:shadow-2xl hover:shadow-fuchsia-500/10">
                <div className="h-64 bg-cover bg-center transition duration-500 group-hover:scale-105" style={{ backgroundImage: `url('${item.image}')` }} />
                <CardContent className="p-6">
                  <Badge className="rounded-full border-0 bg-fuchsia-400/15 text-fuchsia-200 hover:bg-fuchsia-400/15">{item.tag}</Badge>
                  <h3 className="mt-4 text-2xl font-black">{item.name}</h3>
                  <p className="mt-3 leading-7 text-white/68">{item.desc}</p>
                  <div className="mt-5 text-lg font-bold text-cyan-200">Contact for Price</div>
                  <Button asChild className="mt-5 rounded-full bg-white text-slate-950 hover:bg-white/90">
                    <a href="https://wa.me/818076484545" target="_blank" rel="noreferrer">Ask on WhatsApp</a>
                  </Button>
                </CardContent>
              </Card>
            </motion.div>
          ))}
        </div>
      </section>

      <section className="mx-auto grid max-w-7xl gap-6 px-6 py-10 lg:grid-cols-3 lg:px-10">
        {services.map((item) => (
          <Card key={item.title} className="rounded-[2rem] border-white/10 bg-gradient-to-br from-white/8 to-white/5">
            <CardContent className="p-7">
              <div className="inline-flex rounded-3xl bg-white/10 p-4">
                <item.icon className="h-7 w-7" />
              </div>
              <h3 className="mt-5 text-2xl font-black">{item.title}</h3>
              <p className="mt-3 leading-7 text-white/68">{item.text}</p>
            </CardContent>
          </Card>
        ))}
      </section>

      <section id="videos" className="mx-auto max-w-7xl px-6 py-20 lg:px-10">
        <div className="grid gap-6 lg:grid-cols-[0.9fr_1.1fr]">
          <Card className="rounded-[2rem] border-white/10 bg-white/5">
            <CardContent className="p-8">
              <p className="text-sm font-semibold uppercase tracking-[0.3em] text-orange-300/80">Videos</p>
              <h2 className="mt-3 text-4xl font-black">Vehicle video highlights</h2>
              <p className="mt-4 leading-8 text-white/70">
                Your original website included a Videos section. This redesign turns it into a stylish preview area for walkarounds, engine clips, and showroom reels.
              </p>
              <div className="mt-6 space-y-3">
                {videos.map((item) => (
                  <div key={item} className="flex items-center gap-3 rounded-2xl border border-white/10 bg-black/20 px-4 py-4">
                    <PlayCircle className="h-5 w-5 text-orange-300" />
                    <span className="text-white/85">{item}</span>
                  </div>
                ))}
              </div>
            </CardContent>
          </Card>

          <Card className="overflow-hidden rounded-[2rem] border-white/10 bg-white/5">
            <div className="grid h-full md:grid-cols-2">
              <div className="min-h-[340px] bg-cover bg-center" style={{ backgroundImage: "url('https://images.unsplash.com/photo-1503736334956-4c8f8e92946d?auto=format&fit=crop&w=1200&q=80')" }} />
              <CardContent className="flex flex-col justify-center p-8">
                <Badge className="w-fit rounded-full border-0 bg-cyan-400/15 text-cyan-100 hover:bg-cyan-400/15">Showroom media</Badge>
                <h3 className="mt-4 text-3xl font-black">Visual content that sells faster</h3>
                <p className="mt-4 leading-8 text-white/70">
                  Add your real vehicle videos, import reels, bike feature clips, and delivery updates here for a stronger buyer experience.
                </p>
              </CardContent>
            </div>
          </Card>
        </div>
      </section>

      <section id="contact" className="mx-auto max-w-7xl px-6 pb-24 pt-10 lg:px-10">
        <Card className="overflow-hidden rounded-[2rem] border-white/10 bg-gradient-to-r from-orange-500/15 via-fuchsia-500/10 to-cyan-500/15">
          <CardContent className="grid gap-8 p-8 lg:grid-cols-[1fr_0.9fr] lg:p-10">
            <div>
              <p className="text-sm font-semibold uppercase tracking-[0.3em] text-white/70">Contact</p>
              <h2 className="mt-3 text-4xl font-black md:text-5xl">Start your inquiry today</h2>
              <p className="mt-5 max-w-2xl text-lg leading-8 text-white/75">
                Contact Shama Trading for premium vehicles from Japan. Ask about availability, pricing, and updated stock through direct message or phone.
              </p>
            </div>

            <div className="grid gap-4">
              <a href="https://wa.me/818076484545" target="_blank" rel="noreferrer" className="rounded-[1.5rem] border border-white/10 bg-white/10 p-5 transition hover:bg-white/15">
                <div className="flex items-center gap-3">
                  <MessageCircle className="h-6 w-6 text-green-300" />
                  <div>
                    <div className="text-sm text-white/60">WhatsApp</div>
                    <div className="text-xl font-bold">+81 80-7648-4545</div>
                  </div>
                </div>
              </a>
              <a href="tel:+818076484545" className="rounded-[1.5rem] border border-white/10 bg-white/10 p-5 transition hover:bg-white/15">
                <div className="flex items-center gap-3">
                  <Phone className="h-6 w-6 text-cyan-300" />
                  <div>
                    <div className="text-sm text-white/60">Call</div>
                    <div className="text-xl font-bold">+81 80-7648-4545</div>
                  </div>
                </div>
              </a>
              <div className="rounded-[1.5rem] border border-white/10 bg-black/20 p-5">
                <div className="flex items-center gap-3">
                  <Car className="h-6 w-6 text-orange-300" />
                  <Bike className="h-6 w-6 text-fuchsia-300" />
                  <div className="text-white/85">Cars and motorcycles from Japan</div>
                </div>
              </div>
            </div>
          </CardContent>
        </Card>
      </section>
    </div>
  );
}

