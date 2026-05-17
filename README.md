export default function CyberpunkProfile() { const projects = [ { title: 'StegoVault', desc: 'AES-256 + LSB steganography platform for secure hidden communication.', tech: ['Python', 'FastAPI', 'Pillow'], image: 'https://wallpapercave.com/wp/wp5128415.jpg', }, { title: 'Gesture Control', desc: 'Control systems using AI-powered real-time hand gestures.', tech: ['OpenCV', 'MediaPipe', 'Python'], image: 'https://wallpapercave.com/wp/wp9422085.jpg', }, { title: 'NetScan', desc: 'Network reconnaissance dashboard with vulnerability intelligence.', tech: ['Nmap', 'FastAPI', 'Security'], image: 'https://wallpapercave.com/wp/wp2757874.gif', }, ];

return ( <div className="min-h-screen bg-black text-cyan-300 overflow-hidden relative"> <div className="absolute inset-0 bg-[radial-gradient(circle_at_top,rgba(0,255,255,0.15),transparent_40%)]" />

<div className="relative z-10 max-w-7xl mx-auto px-6 py-10 grid lg:grid-cols-[320px_1fr] gap-8">
    {/* Sidebar */}
    <div className="space-y-6">
      <div className="bg-[#071018]/80 border border-cyan-500/30 rounded-3xl p-6 shadow-[0_0_40px_rgba(0,255,255,0.15)] backdrop-blur-xl">
        <div className="relative">
          <img
            src="https://wallpapercave.com/wp/wp9422179.jpg"
            className="w-44 h-44 rounded-full object-cover mx-auto border-4 border-cyan-400 shadow-[0_0_30px_cyan]"
          />
          <div className="absolute bottom-3 right-16 w-5 h-5 rounded-full bg-green-400 animate-pulse" />
        </div>

        <h1 className="text-4xl font-bold text-center mt-6 tracking-wide text-cyan-200">
          Anubhav Pati
        </h1>

        <p className="text-center text-cyan-500 mt-2 text-sm">
          Full Stack Developer • Cybersecurity Enthusiast
        </p>

        <div className="mt-6 border border-cyan-500/20 rounded-2xl p-4 bg-black/40">
          <p className="text-green-400 font-mono text-sm">$ whoami</p>
          <p className="mt-3 text-sm leading-7 text-cyan-100/80">
            Building secure systems, AI-powered tools and futuristic
            digital experiences.
          </p>
        </div>

        <div className="mt-6 space-y-3 text-sm">
          {[
            'Arch Linux',
            'FastAPI',
            'Computer Vision',
            'Web3',
          ].map((item) => (
            <div
              key={item}
              className="border border-cyan-500/20 rounded-xl px-4 py-3 bg-black/30 hover:bg-cyan-500/10 transition"
            >
              ✦ {item}
            </div>
          ))}
        </div>
      </div>

      <div className="bg-[#071018]/80 border border-cyan-500/30 rounded-3xl p-6 backdrop-blur-xl">
        <h2 className="text-xl font-semibold mb-5 text-cyan-200">
          Connect
        </h2>

        <div className="space-y-4">
          {['LinkedIn', 'Instagram', 'GitHub', 'Discord'].map((link) => (
            <div
              key={link}
              className="border border-cyan-500/20 rounded-xl px-4 py-3 hover:bg-cyan-500/10 transition cursor-pointer"
            >
              {link}
            </div>
          ))}
        </div>
      </div>
    </div>

    {/* Main */}
    <div className="space-y-8">
      {/* Hero */}
      <div className="relative rounded-[32px] overflow-hidden border border-cyan-500/30 shadow-[0_0_50px_rgba(0,255,255,0.15)]">
        <img
          src="https://images.alphacoders.com/133/1330719.jpeg"
          className="w-full h-[420px] object-cover opacity-50"
        />

        <div className="absolute inset-0 bg-gradient-to-r from-black via-black/80 to-transparent" />

        <div className="absolute inset-0 flex flex-col justify-center px-10 lg:px-16">
          <p className="text-green-400 font-mono mb-4 text-sm">
            &gt; initialize_profile.exe
          </p>

          <h1 className="text-5xl lg:text-7xl font-black leading-tight text-white max-w-3xl">
            Welcome to <span className="text-cyan-400">Anubhav's</span>{' '}
            Digital World
          </h1>

          <p className="mt-6 text-cyan-100/70 max-w-2xl text-lg leading-8">
            Anime Coder • Cyberpunk Developer • Digital Dreamer • Terminal Addict
          </p>

          <div className="flex flex-wrap gap-4 mt-8">
            <button className="px-6 py-3 rounded-2xl bg-cyan-400 text-black font-bold hover:scale-105 transition">
              Explore Projects
            </button>

            <button className="px-6 py-3 rounded-2xl border border-cyan-400 text-cyan-300 hover:bg-cyan-400/10 transition">
              Connect With Me
            </button>
          </div>
        </div>
      </div>

      {/* About */}
      <div className="bg-[#071018]/80 rounded-[32px] border border-cyan-500/30 p-8 backdrop-blur-xl">
        <div className="flex items-center justify-between flex-wrap gap-6">
          <div>
            <p className="text-green-400 font-mono text-sm">
              &gt; about_me.md
            </p>
            <h2 className="text-4xl font-bold mt-3 text-cyan-100">
              About Me
            </h2>
          </div>

          <img
            src="https://media.tenor.com/oqKH9I7k0SAAAAAC/anime-computer.gif"
            className="w-40 rounded-2xl border border-cyan-500/20"
          />
        </div>

        <p className="mt-8 text-cyan-100/70 leading-8 text-lg">
          Passionate developer focused on building immersive, scalable,
          and futuristic systems. I love cybersecurity, Linux,
          automation, and experimenting with AI-powered ideas.
        </p>

        <div className="grid md:grid-cols-4 gap-5 mt-10">
          {[
            'Problem Solver',
            'CTF Player',
            'AI Builder',
            'Open Source',
          ].map((item) => (
            <div
              key={item}
              className="rounded-2xl border border-cyan-500/20 bg-black/30 p-5 text-center hover:-translate-y-2 transition"
            >
              <div className="text-3xl mb-3">⚡</div>
              <p>{item}</p>
            </div>
          ))}
        </div>
      </div>

      {/* Projects */}
      <div className="bg-[#071018]/80 rounded-[32px] border border-cyan-500/30 p-8 backdrop-blur-xl">
        <p className="text-green-400 font-mono text-sm">
          &gt; featured_projects.sh
        </p>

        <h2 className="text-4xl font-bold mt-3 text-cyan-100">
          Featured Projects
        </h2>

        <div className="grid lg:grid-cols-3 gap-6 mt-10">
          {projects.map((project) => (
            <div
              key={project.title}
              className="rounded-3xl overflow-hidden border border-cyan-500/20 bg-black/40 hover:-translate-y-3 transition duration-300 group"
            >
              <div className="overflow-hidden">
                <img
                  src={project.image}
                  className="h-52 w-full object-cover group-hover:scale-110 transition duration-500"
                />
              </div>

              <div className="p-6">
                <h3 className="text-2xl font-bold text-cyan-200">
                  {project.title}
                </h3>

                <p className="mt-3 text-cyan-100/60 leading-7 text-sm">
                  {project.desc}
                </p>

                <div className="flex flex-wrap gap-2 mt-5">
                  {project.tech.map((tech) => (
                    <span
                      key={tech}
                      className="px-3 py-1 rounded-full text-xs bg-cyan-500/10 border border-cyan-500/20"
                    >
                      {tech}
                    </span>
                  ))}
                </div>
              </div>
            </div>
          ))}
        </div>
      </div>

      {/* Footer */}
      <div className="rounded-[32px] border border-cyan-500/20 bg-black/40 p-8 text-center">
        <img
          src="https://media.tenor.com/qJ5evVs-_uUAAAAC/coding-anime.gif"
          className="mx-auto w-72 rounded-2xl border border-cyan-500/20"
        />

        <p className="mt-8 text-2xl text-cyan-300 font-mono">
          Lost in code. Living in neon. ⚡
        </p>

        <p className="mt-3 text-cyan-100/50">
          connection terminated... see you in cyberspace.
        </p>
      </div>
    </div>
  </div>
</div>

); }
