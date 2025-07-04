import React, { useState } from "react"; import { motion } from "framer-motion"; import { Button } from "@/components/ui/button"; import { Dialog, DialogContent } from "@/components/ui/dialog";

const prizes = [ { label: "299 Recharge", color: "bg-red-400" }, { label: "2GB DATA", color: "bg-green-400" }, { label: "5GB DATA", color: "bg-yellow-400" }, { label: "1GB DATA", color: "bg-blue-400" }, ];

export default function SpinWheelGame() { const [rotating, setRotating] = useState(false); const [rotation, setRotation] = useState(0); const [selectedPrize, setSelectedPrize] = useState(null); const [showModal, setShowModal] = useState(false);

const spin = () => { const randomIndex = Math.floor(Math.random() * prizes.length); const anglePerSlice = 360 / prizes.length; const newRotation = 360 * 5 + randomIndex * anglePerSlice;

setRotating(true);
setRotation(newRotation);

setTimeout(() => {
  setSelectedPrize(prizes[randomIndex]);
  setShowModal(true);
  setRotating(false);
}, 3000);

};

return ( <div className="flex flex-col items-center justify-center min-h-screen bg-gradient-to-b from-slate-700 to-slate-900 text-white"> <div className="relative w-64 h-64 rounded-full border-[6px] border-cyan-400 overflow-hidden"> <motion.div className="absolute w-full h-full origin-center" animate={{ rotate: rotation }} transition={{ duration: 3, ease: "easeOut" }} > {prizes.map((prize, i) => { const angle = i * (360 / prizes.length); return ( <div key={i} className={absolute w-1/2 h-1/2 top-0 left-1/2 ${prize.color} flex items-center justify-center text-black font-bold text-xs} style={{ transform: rotate(${angle}deg), transformOrigin: '0% 100%' }} > <div style={{ transform: rotate(-${angle}deg) }}>{prize.label}</div> </div> ); })} </motion.div> <div className="absolute inset-0 flex items-center justify-center"> <Button
className="z-10 bg-black text-white px-4 py-2 rounded-full text-lg"
onClick={spin}
disabled={rotating}
> Spin </Button> </div> </div>

<Dialog open={showModal} onOpenChange={setShowModal}>
    <DialogContent className="text-center p-6">
      <h2 className="text-2xl font-bold mb-4">আপুনি জিকাৰিছে:</h2>
      <p className="text-xl mb-6">🎁 {selectedPrize?.label}</p>
      <p className="mb-4">এই উপহাৰটো লাভ কৰিবলৈ তলৰ কামটো সম্পূৰ্ণ কৰক:</p>
      <a
        href="https://instagram.com/akhim_b18"
        target="_blank"
        rel="noopener noreferrer"
        className="inline-block bg-pink-500 text-white px-6 py-2 rounded-lg hover:bg-pink-600 transition"
      >
        Follow on Instagram
      </a>
    </DialogContent>
  </Dialog>
</div>

); }

