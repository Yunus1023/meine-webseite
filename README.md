# meine-webseite

import { BrowserRouter as Router, Routes, Route, Link } from "react-router-dom";


    <div className="p-4 text-center">
      <h1 className="text-3xl font-bold">Willkommen auf meiner Website!</h1>
      <p className="mt-2">Hier erfährst du mehr über mich.</p>
    </div>
  );
}


    <div className="p-4">
      <h2 className="text-2xl font-semibold">⚽ Fußball</h2>
      <p className="mt-2">Ich spiele als Mittelfeldspieler bei SPG KUMMA U18.</p>
    </div>
  );
}


    <div className="p-4">
      <h2 className="text-2xl font-semibold">📚 Schule</h2>
      <p className="mt-2">Ich bin Schüler und interessiere mich besonders für Wissen und Bücher.</p>
    </div>
  );
}


    <div className="p-4">
      <h2 className="text-2xl font-semibold">🎯 Hobbys</h2>
      <p className="mt-2">Ich lese gerne, trainiere viel und höre Rap/Pop-Songs.</p>
    </div>
  );
}


    <nav className="p-4 bg-gray-800 text-white flex gap-4">
      <Link to="/">Home</Link>
      <Link to="/football">Fußball</Link>
      <Link to="/school">Schule</Link>
      <Link to="/hobbies">Hobbys</Link>
    </nav>
  );
}

export default function App() {
  return (
    <Router>
      <Navbar />
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/football" element={<Football />} />
        <Route path="/school" element={<School />} />
        <Route path="/hobbies" element={<Hobbies />} />
      </Routes>
    </Router>
  );
}
