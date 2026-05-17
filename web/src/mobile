export default function MobileCollabUI() {
  const rooms = [
    {
      name: 'Frontend Team',
      members: 12,
      status: 'Active',
    },
    {
      name: 'Backend API',
      members: 7,
      status: 'Discussion',
    },
    {
      name: 'UI Research',
      members: 4,
      status: 'Review',
    },
  ];

  return (
    <div className="min-h-screen bg-zinc-950 text-white flex flex-col">
      {/* Header */}
      <header className="sticky top-0 z-20 bg-zinc-950/80 backdrop-blur border-b border-zinc-800 px-4 py-4 flex items-center justify-between">
        <div>
          <h1 className="text-2xl font-bold tracking-tight">Ko-Lab</h1>
          <p className="text-sm text-zinc-400">Collaborative Workspace</p>
        </div>

        <div className="w-11 h-11 rounded-full bg-gradient-to-br from-indigo-500 to-cyan-400 flex items-center justify-center font-bold shadow-lg">
          S
        </div>
      </header>

      {/* Search */}
      <div className="px-4 pt-4">
        <div className="bg-zinc-900 border border-zinc-800 rounded-2xl px-4 py-3 flex items-center gap-3 shadow-lg">
          <span className="text-zinc-500">🔍</span>
          <input
            type="text"
            placeholder="Search rooms, members, projects..."
            className="bg-transparent outline-none w-full text-sm placeholder:text-zinc-500"
          />
        </div>
      </div>

      {/* Banner */}
      <section className="px-4 pt-5">
        <div className="rounded-3xl bg-gradient-to-br from-indigo-600 via-purple-600 to-cyan-500 p-5 shadow-2xl overflow-hidden relative">
          <div className="absolute top-0 right-0 w-32 h-32 bg-white/10 rounded-full blur-2xl" />

          <div className="relative z-10">
            <p className="text-sm text-white/80 mb-2">Workspace Overview</p>
            <h2 className="text-2xl font-bold leading-tight mb-3">
              Build Together.
              <br />
              Collaborate Faster.
            </h2>

            <button className="mt-2 bg-white text-black px-5 py-2 rounded-xl font-semibold text-sm shadow-lg active:scale-95 transition">
              Open Workspace
            </button>
          </div>
        </div>
      </section>

      {/* Stats */}
      <section className="grid grid-cols-2 gap-4 px-4 pt-5">
        <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-4 shadow-lg">
          <p className="text-zinc-400 text-sm">Active Rooms</p>
          <h3 className="text-3xl font-bold mt-2">12</h3>
        </div>

        <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-4 shadow-lg">
          <p className="text-zinc-400 text-sm">Online Members</p>
          <h3 className="text-3xl font-bold mt-2">38</h3>
        </div>
      </section>

      {/* Rooms */}
      <section className="px-4 pt-6 flex-1 pb-28">
        <div className="flex items-center justify-between mb-4">
          <h2 className="text-xl font-semibold">Your Rooms</h2>
          <button className="text-sm text-cyan-400">See all</button>
        </div>

        <div className="space-y-4">
          {rooms.map((room, index) => (
            <div
              key={index}
              className="bg-zinc-900 border border-zinc-800 rounded-3xl p-4 shadow-lg active:scale-[0.98] transition"
            >
              <div className="flex items-start justify-between">
                <div>
                  <h3 className="font-semibold text-lg">{room.name}</h3>
                  <p className="text-zinc-400 text-sm mt-1">
                    {room.members} Members
                  </p>
                </div>

                <div className="bg-cyan-500/15 text-cyan-400 text-xs px-3 py-1 rounded-full border border-cyan-500/20">
                  {room.status}
                </div>
              </div>

              <div className="flex items-center justify-between mt-5">
                <div className="flex -space-x-2">
                  <div className="w-8 h-8 rounded-full bg-indigo-500 border-2 border-zinc-900" />
                  <div className="w-8 h-8 rounded-full bg-pink-500 border-2 border-zinc-900" />
                  <div className="w-8 h-8 rounded-full bg-cyan-500 border-2 border-zinc-900" />
                </div>

                <button className="bg-white text-black px-4 py-2 rounded-xl text-sm font-semibold active:scale-95 transition">
                  Open
                </button>
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* Floating Button */}
      <button className="fixed bottom-24 right-5 w-16 h-16 rounded-2xl bg-gradient-to-br from-indigo-500 to-cyan-400 text-3xl shadow-2xl active:scale-95 transition">
        +
      </button>

      {/* Bottom Navigation */}
      <nav className="fixed bottom-0 left-0 right-0 bg-zinc-950/90 backdrop-blur border-t border-zinc-800 px-4 py-3 flex items-center justify-around">
        <button className="flex flex-col items-center text-cyan-400 text-sm">
          <span className="text-xl">🏠</span>
          Home
        </button>

        <button className="flex flex-col items-center text-zinc-500 text-sm">
          <span className="text-xl">💬</span>
          Chat
        </button>

        <button className="flex flex-col items-center text-zinc-500 text-sm">
          <span className="text-xl">📁</span>
          Projects
        </button>

        <button className="flex flex-col items-center text-zinc-500 text-sm">
          <span className="text-xl">👤</span>
          Profile
        </button>
      </nav>
    </div>
  );
}
