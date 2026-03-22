import React from 'react';
import { motion } from 'framer-motion';
import { BookOpen, PlayCircle, Download, Bell, ShieldCheck, CreditCard, Users, MessageCircle, CheckCircle2, Star } from 'lucide-react';
import { Card, CardContent } from '@/components/ui/card';
import { Button } from '@/components/ui/button';

const features = [
  {
    icon: PlayCircle,
    title: 'Live & Recorded Classes',
    desc: 'Students can join live sessions and access structured recorded chapter-wise lectures anytime from any device.',
  },
  {
    icon: Download,
    title: 'Study Materials & PDFs',
    desc: 'Upload notes, practice sheets, assignments, and premium downloadable study resources.',
  },
  {
    icon: CreditCard,
    title: 'Secure Online Payments',
    desc: 'Accept UPI, debit card, credit card, and net banking payments for courses and materials.',
  },
  {
    icon: Bell,
    title: 'Instant Updates',
    desc: 'Share class notices, exam alerts, new batch launches, and important announcements instantly.',
  },
  {
    icon: Users,
    title: 'Student Dashboard',
    desc: 'A personalized dashboard for purchased courses, lessons, downloads, and progress tracking.',
  },
  {
    icon: MessageCircle,
    title: 'Exam-Focused Guidance',
    desc: 'Targeted support for Math and Reasoning preparation with student-friendly guidance for government exams.',
  },
];

const courses = [
  {
    title: 'SSC & CGL Math Batch',
    price: '₹1,999',
    points: ['Live + recorded classes', 'PDF notes included', 'Government exam practice sets'],
  },
  {
    title: 'Reasoning Master Course',
    price: '₹3,499',
    points: ['Reasoning shortcuts and concepts', 'Mock tests and revision support', 'SSC, CGL and exam updates'],
  },
  {
    title: 'Railway & State Exam Pack',
    price: '₹999',
    points: ['Downloadable notes', 'Railway and state exam content', 'Useful for revision and self-study'],
  },
];

const testimonials = [
  {
    name: 'Aarav',
    text: 'The dashboard is super easy to use. I got my classes and notes right after payment.',
  },
  {
    name: 'Sneha',
    text: 'Very organized platform. Announcements, videos, and PDFs are all in one place.',
  },
  {
    name: 'Rohit',
    text: 'The course flow feels professional and the study material is easy to access anytime.',
  },
];

export default function EdTechWebsitePreview() {
  return (
    <div className="min-h-screen bg-slate-50 text-slate-900">
      <header className="sticky top-0 z-50 border-b border-slate-200 bg-white/90 backdrop-blur">
        <div className="mx-auto flex max-w-7xl items-center justify-between px-6 py-4">
          <div className="flex items-center gap-2">
            <div className="rounded-2xl bg-slate-900 p-2 text-white">
              <BookOpen className="h-5 w-5" />
            </div>
            <div>
              <p className="text-lg font-bold">Mizoram Education Hub</p>
              <p className="text-xs text-slate-500">Learning with Dharampal Yadav</p>
            </div>
          </div>
          <nav className="hidden items-center gap-6 text-sm font-medium md:flex">
            <a href="#home" className="hover:text-slate-600">Home</a>
            <a href="#courses" className="hover:text-slate-600">Courses</a>
            <a href="#features" className="hover:text-slate-600">Features</a>
            <a href="#exams" className="hover:text-slate-600">Exams</a>
            <a href="#testimonials" className="hover:text-slate-600">Reviews</a>
            <a href="#contact" className="hover:text-slate-600">Contact</a>
          </nav>
          <div className="flex items-center gap-3">
            <Button variant="outline" className="rounded-2xl">Login</Button>
            <Button className="rounded-2xl">Enroll Now</Button>
          </div>
        </div>
      </header>

      <section id="home" className="relative overflow-hidden">
        <div className="mx-auto grid max-w-7xl gap-10 px-6 py-20 md:grid-cols-2 md:py-28">
          <motion.div
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.6 }}
            className="flex flex-col justify-center"
          >
            <div className="mb-4 inline-flex w-fit items-center gap-2 rounded-full border border-slate-200 bg-white px-4 py-2 text-sm shadow-sm">
              <ShieldCheck className="h-4 w-4" /> Trusted coaching for government exam aspirants
            </div>
            <h1 className="text-4xl font-black leading-tight tracking-tight md:text-6xl">
              Your Trusted Coaching Platform for SSC, CGL, Railways & State Exams
            </h1>
            <p className="mt-6 max-w-xl text-lg leading-8 text-slate-600">
              Mizoram Education Hub by Dharampal Yadav offers expert Math and Reasoning classes, study materials, live and recorded lectures, exam-focused updates, and a smooth learning experience for competitive exam aspirants.
            </p>
            <div className="mt-8 flex flex-wrap gap-4">
              <Button size="lg" className="rounded-2xl px-6">Explore Courses</Button>
              <Button size="lg" variant="outline" className="rounded-2xl px-6">Watch Demo</Button>
            </div>
            <div className="mt-8 flex flex-wrap items-center gap-6 text-sm text-slate-600">
              <div className="flex items-center gap-2"><CheckCircle2 className="h-4 w-4" /> Math & Reasoning focus</div>
              <div className="flex items-center gap-2"><CheckCircle2 className="h-4 w-4" /> Live + recorded classes</div>
              <div className="flex items-center gap-2"><CheckCircle2 className="h-4 w-4" /> SSC, CGL & Railways prep</div>
            </div>
          </motion.div>

          <motion.div
            initial={{ opacity: 0, scale: 0.96 }}
            animate={{ opacity: 1, scale: 1 }}
            transition={{ duration: 0.7 }}
            className="relative"
          >
            <div className="rounded-[2rem] border border-slate-200 bg-white p-5 shadow-2xl">
              <div className="grid gap-4">
                <Card className="rounded-2xl border-slate-200 shadow-sm">
                  <CardContent className="p-5">
                    <div className="flex items-center justify-between">
                      <div>
                        <p className="text-sm text-slate-500">Student Dashboard</p>
                        <h3 className="text-xl font-bold">Welcome back, Student</h3>
                      </div>
                      <div className="rounded-2xl bg-slate-100 p-3">
                        <Users className="h-5 w-5" />
                      </div>
                    </div>
                    <div className="mt-5 grid gap-3 sm:grid-cols-3">
                      <div className="rounded-2xl bg-slate-50 p-4">
                        <p className="text-sm text-slate-500">Purchased</p>
                        <p className="text-2xl font-bold">08</p>
                      </div>
                      <div className="rounded-2xl bg-slate-50 p-4">
                        <p className="text-sm text-slate-500">Videos</p>
                        <p className="text-2xl font-bold">124</p>
                      </div>
                      <div className="rounded-2xl bg-slate-50 p-4">
                        <p className="text-sm text-slate-500">Downloads</p>
                        <p className="text-2xl font-bold">36</p>
                      </div>
                    </div>
                  </CardContent>
                </Card>

                <div className="grid gap-4 md:grid-cols-2">
                  <Card className="rounded-2xl border-slate-200 shadow-sm">
                    <CardContent className="p-5">
                      <div className="mb-3 flex items-center gap-2">
                        <PlayCircle className="h-5 w-5" />
                        <h4 className="font-semibold">Latest Lecture</h4>
                      </div>
                      <p className="text-sm text-slate-600">Chapter-wise recorded class with resume playback support.</p>
                    </CardContent>
                  </Card>
                  <Card className="rounded-2xl border-slate-200 shadow-sm">
                    <CardContent className="p-5">
                      <div className="mb-3 flex items-center gap-2">
                        <Bell className="h-5 w-5" />
                        <h4 className="font-semibold">New Announcement</h4>
                      </div>
                      <p className="text-sm text-slate-600">New batch updates and exam notices are posted here for enrolled students.</p>
                    </CardContent>
                  </Card>
                </div>
              </div>
            </div>
          </motion.div>
        </div>
      </section>

      <section id="exams" className="mx-auto max-w-7xl px-6 pt-6 pb-8">
        <div className="rounded-[2rem] border border-slate-200 bg-white p-8 shadow-sm">
          <p className="text-sm font-semibold uppercase tracking-[0.2em] text-slate-500">Exam Categories</p>
          <h2 className="mt-3 text-3xl font-black md:text-4xl">Focused preparation for top government exams</h2>
          <div className="mt-6 grid gap-4 sm:grid-cols-2 lg:grid-cols-4">
            {['SSC', 'CGL', 'Railways', 'State Exams'].map((exam) => (
              <div key={exam} className="rounded-2xl bg-slate-50 p-5 text-center text-lg font-semibold">{exam}</div>
            ))}
          </div>
        </div>
      </section>

      <section id="features" className="mx-auto max-w-7xl px-6 py-16">
        <div className="mb-10 max-w-2xl">
          <p className="text-sm font-semibold uppercase tracking-[0.2em] text-slate-500">Core Features</p>
          <h2 className="mt-3 text-3xl font-black md:text-4xl">Everything needed for a modern teaching business</h2>
          <p className="mt-4 text-slate-600">Designed for teachers who want to teach, sell, update, and support students in one smooth ecosystem.</p>
        </div>
        <div className="grid gap-6 md:grid-cols-2 xl:grid-cols-3">
          {features.map((feature, index) => {
            const Icon = feature.icon;
            return (
              <motion.div
                key={feature.title}
                initial={{ opacity: 0, y: 20 }}
                whileInView={{ opacity: 1, y: 0 }}
                viewport={{ once: true }}
                transition={{ duration: 0.4, delay: index * 0.05 }}
              >
                <Card className="h-full rounded-[1.5rem] border-slate-200 shadow-sm transition hover:-translate-y-1 hover:shadow-lg">
                  <CardContent className="p-6">
                    <div className="mb-4 w-fit rounded-2xl bg-slate-100 p-3">
                      <Icon className="h-6 w-6" />
                    </div>
                    <h3 className="text-xl font-bold">{feature.title}</h3>
                    <p className="mt-3 leading-7 text-slate-600">{feature.desc}</p>
                  </CardContent>
                </Card>
              </motion.div>
            );
          })}
        </div>
      </section>

      <section id="courses" className="bg-white py-16">
        <div className="mx-auto max-w-7xl px-6">
          <div className="mb-10 flex flex-col justify-between gap-4 md:flex-row md:items-end">
            <div>
              <p className="text-sm font-semibold uppercase tracking-[0.2em] text-slate-500">Popular Courses</p>
              <h2 className="mt-3 text-3xl font-black md:text-4xl">Professional course catalog section</h2>
            </div>
            <Button variant="outline" className="w-fit rounded-2xl">View All Courses</Button>
          </div>
          <div className="grid gap-6 md:grid-cols-3">
            {courses.map((course) => (
              <Card key={course.title} className="rounded-[1.75rem] border-slate-200 shadow-sm">
                <CardContent className="p-6">
                  <div className="flex items-start justify-between gap-4">
                    <div>
                      <h3 className="text-xl font-bold">{course.title}</h3>
                      <p className="mt-2 text-3xl font-black">{course.price}</p>
                    </div>
                    <div className="rounded-2xl bg-slate-100 p-3">
                      <BookOpen className="h-5 w-5" />
                    </div>
                  </div>
                  <div className="mt-6 space-y-3">
                    {course.points.map((point) => (
                      <div key={point} className="flex items-center gap-2 text-sm text-slate-600">
                        <CheckCircle2 className="h-4 w-4" /> {point}
                      </div>
                    ))}
                  </div>
                  <Button className="mt-6 w-full rounded-2xl">Buy Now</Button>
                </CardContent>
              </Card>
            ))}
          </div>
        </div>
      </section>

      <section id="testimonials" className="mx-auto max-w-7xl px-6 py-16">
        <div className="mb-10 max-w-2xl">
          <p className="text-sm font-semibold uppercase tracking-[0.2em] text-slate-500">Student Feedback</p>
          <h2 className="mt-3 text-3xl font-black md:text-4xl">Built to feel trustworthy and easy</h2>
        </div>
        <div className="grid gap-6 md:grid-cols-3">
          {testimonials.map((item) => (
            <Card key={item.name} className="rounded-[1.75rem] border-slate-200 shadow-sm">
              <CardContent className="p-6">
                <div className="mb-4 flex gap-1">
                  {Array.from({ length: 5 }).map((_, i) => (
                    <Star key={i} className="h-4 w-4 fill-current" />
                  ))}
                </div>
                <p className="leading-7 text-slate-600">“{item.text}”</p>
                <p className="mt-5 font-semibold">{item.name}</p>
              </CardContent>
            </Card>
          ))}
        </div>
      </section>

      <section id="contact" className="bg-slate-900 py-16 text-white">
        <div className="mx-auto grid max-w-7xl gap-8 px-6 md:grid-cols-2 md:items-center">
          <div>
            <p className="text-sm font-semibold uppercase tracking-[0.2em] text-slate-300">Get Started</p>
            <h2 className="mt-3 text-3xl font-black md:text-5xl">Launch your teaching platform with a premium online presence.</h2>
            <p className="mt-4 max-w-xl text-slate-300">
              Built for Mizoram Education Hub to deliver a professional platform with live classes, recorded lessons, secure payments, and student-friendly navigation.
            </p>
          </div>
          <Card className="rounded-[2rem] border-white/10 bg-white text-slate-900 shadow-xl">
            <CardContent className="p-6">
              <h3 className="text-2xl font-bold">Book a Demo</h3>
              <p className="mt-2 text-slate-600">Show students your classes, notes, and paid courses in one organized place.</p>
              <div className="mt-6 grid gap-3">
                <input className="rounded-2xl border border-slate-200 px-4 py-3 outline-none" placeholder="Your Name" />
                <input className="rounded-2xl border border-slate-200 px-4 py-3 outline-none" placeholder="Phone Number" />
                <input className="rounded-2xl border border-slate-200 px-4 py-3 outline-none" placeholder="Email Address" defaultValue="8131959163@unknown.email" />
                <input className="rounded-2xl border border-slate-200 px-4 py-3 outline-none" placeholder="Phone / WhatsApp" defaultValue="8131959163" />
                <Button className="rounded-2xl">Request Callback</Button>
              </div>
            </CardContent>
          </Card>
        </div>
      </section>
    </div>
  );
}
