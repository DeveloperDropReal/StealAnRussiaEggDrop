@import url('https://fonts.googleapis.com/css2?family=Creepster&family=Montserrat:wght@400;600;700;900&display=swap');

/* Main Document Styles */
body {
    background-color: #0b0612;
    color: #e2e8f0;
    font-family: 'Montserrat', sans-serif;
    overflow-x: hidden;
    background-image: 
        radial-gradient(circle at 10% 20%, rgba(255, 102, 0, 0.08) 0%, transparent 20%),
        radial-gradient(circle at 90% 80%, rgba(139, 92, 246, 0.1) 0%, transparent 25%),
        radial-gradient(circle at 50% 50%, rgba(15, 8, 28, 0.8) 0%, #0b0612 100%);
}

/* Header Text Effects */
.title-glow {
    font-family: 'Creepster', cursive;
    text-shadow: 0 0 10px #ff6600, 0 0 20px #ff6600, 0 0 40px #8b5cf6;
}

/* Case Box Hover & Glow Effects */
.box-glow-orange {
    box-shadow: 0 0 20px rgba(255, 102, 0, 0.25);
    transition: all 0.3s ease;
}
.box-glow-orange:hover {
    box-shadow: 0 0 30px rgba(255, 102, 0, 0.5);
    transform: translateY(-2px);
}

.box-glow-purple {
    box-shadow: 0 0 20px rgba(139, 92, 246, 0.25);
    transition: all 0.3s ease;
}
.box-glow-purple:hover {
    box-shadow: 0 0 30px rgba(139, 92, 246, 0.5);
    transform: translateY(-2px);
}

/* Roulette Reel Container & Pointer */
.roulette-container {
    position: relative;
    overflow: hidden;
    width: 100%;
    height: 160px;
}

.roulette-pointer {
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 4px;
    height: 100%;
    background: #ff6600;
    box-shadow: 0 0 15px #ff6600, 0 0 5px #ffffff;
    z-index: 20;
}

.roulette-track {
    display: flex;
    position: absolute;
    left: 0;
    top: 10px;
    height: 140px;
    will-change: transform;
    transition: transform 0s cubic-bezier(0.15, 0.9, 0.2, 1);
}

/* Custom Scrollbar */
::-webkit-scrollbar {
    width: 8px;
}
::-webkit-scrollbar-track {
    background: #0b0612;
}
::-webkit-scrollbar-thumb {
    background: #2d184c;
    border-radius: 4px;
}
::-webkit-scrollbar-thumb:hover {
    background: #ff6600;
}

/* Floating Animations */
@keyframes float {
    0%, 100% { transform: translateY(0px) rotate(0deg); }
    50% { transform: translateY(-8px) rotate(3deg); }
}

.animate-float {
    animation: float 4s ease-in-out infinite;
}