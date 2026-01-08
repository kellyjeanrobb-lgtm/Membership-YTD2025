<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Membership Dashboard - 2025</title>
    
    <!-- 1. Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- 2. Load React and ReactDOM -->
    <script src="https://unpkg.com/react@18.2.0/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@18.2.0/umd/react-dom.production.min.js"></script>
    
    <!-- 3. Load PropTypes (Required dependency for Recharts) -->
    <script src="https://unpkg.com/prop-types/prop-types.min.js"></script>
    
    <!-- 4. Load Recharts -->
    <script src="https://unpkg.com/recharts@2.12.7/umd/Recharts.js"></script>
    
    <!-- 5. Load Babel for JSX -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

    <style>
        body { background-color: #f8fafc; }
        /* Custom scrollbar for cleaner look */
        ::-webkit-scrollbar { width: 6px; height: 6px; }
        ::-webkit-scrollbar-track { background: transparent; }
        ::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 3px; }
        .no-scrollbar::-webkit-scrollbar { display: none; }
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        // Access Recharts from the global window object
        const { 
            BarChart, Bar, LineChart, Line, ComposedChart, Area, AreaChart, PieChart, Pie,
            XAxis, YAxis, CartesianGrid, Tooltip, Legend, ResponsiveContainer, 
            Cell, ReferenceLine, LabelList 
        } = Recharts;

        // --- ICON COMPONENTS ---
        const IconBase = ({ d, color, className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={`${className || ''} ${color || ''}`}>
                <path d={d} />
            </svg>
        );

        const Users = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>;
        const DollarSign = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>;
        const Activity = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>;
        const FileText = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>;
        const UserMinus = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><line x1="22" y1="11" x2="16" y2="11"/></svg>;
        const UserPlus = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><line x1="19" y1="8" x2="19" y2="14"/><line x1="22" y1="11" x2="16" y2="11"/></svg>;
        const TrendingDown = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polyline points="23 18 13.5 8.5 8.5 13.5 1 6"/><polyline points="17 18 23 18 23 12"/></svg>;
        const TrendingUp = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polyline points="23 6 13.5 15.5 8.5 10.5 1 18"/><polyline points="17 6 23 6 23 12"/></svg>;
        const Wallet = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M20 12V8H6a2 2 0 0 1-2-2c0-1.1.9-2 2-2h12v4"/><path d="M4 6v12a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2H6a2 2 0 0 0-2 2z"/></svg>;
        const CheckCircle = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>;
        const FileCheck = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/><polyline points="14 2 14 8 20 8"/><path d="m9 15 2 2 4-4"/></svg>;
        const ClipboardList = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"/><rect x="8" y="2" width="8" height="4" rx="1" ry="1"/><path d="M12 11h4"/><path d="M12 16h4"/><path d="M8 11h.01"/><path d="M8 16h.01"/></svg>;
        const UserCheck = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><polyline points="16 11 18 13 22 9"/></svg>;
        const ArrowRightLeft = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="m16 3 4 4-4 4"/><path d="M20 7H4"/><path d="m8 21-4-4 4-4"/><path d="M4 17h16"/></svg>;
        const Layers = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polygon points="12 2 2 7 12 12 22 7 12 2"/><polyline points="2 17 12 22 22 17"/><polyline points="2 12 12 17 22 12"/></svg>;
        const BarChart3 = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><line x1="12" y1="20" x2="12" y2="10"/><line x1="18" y1="20" x2="18" y2="4"/><line x1="6" y1="20" x2="6" y2="16"/></svg>;
        const Clock = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>;
        const AlertCircle = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>;
        const BookOpen = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>;
        const Info = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="10"/><line x1="12" y1="16" x2="12" y2="12"/><line x1="12" y1="8" x2="12.01" y2="8"/></svg>;
        const MapPin = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>;
        const Calendar = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>;
        const User = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"/><circle cx="12" cy="7" r="4"/></svg>;
        const Database = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M21 12c0 1.66-4 3-9 3s-9-1.34-9-3"/><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5"/></svg>;
        const ArrowRight = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>;
        const ArrowDown = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><line x1="12" y1="5" x2="12" y2="19"/><polyline points="19 12 12 19 5 12"/></svg>;
        const RefreshCw = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polyline points="23 4 23 10 17 10"/><polyline points="1 20 1 14 7 14"/><path d="M3.51 9a9 9 0 0 1 14.85-3.36L23 10M1 14l4.64 4.36A9 9 0 0 0 20.49 15"/></svg>;
        const Star = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/></svg>;
        const Settings = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>;
        const Target = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="6"/><circle cx="12" cy="12" r="2"/></svg>;
        const Zap = (p) => <svg {...p} xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"/></svg>;

        const PipelineCycleInfographic = () => {
            return (
                <div className="w-full bg-white rounded-xl border border-slate-200 shadow-sm p-6 relative">
                    <h3 className="font-bold text-slate-900 mb-8 text-center text-xl">Membership Lifecycle & Ecosystem</h3>
                    
                    <div className="flex flex-col lg:flex-row items-center justify-center gap-8 lg:gap-12 relative z-10">
                        
                        {/* 1. THE FUNNEL (LEFT) */}
                        <div className="flex flex-col items-center w-full max-w-xs">
                            <div className="text-sm font-bold text-slate-400 uppercase tracking-widest mb-2">Acquisition Pipeline</div>
                            <div className="w-full space-y-1">
                                {/* Applicants */}
                                <div className="bg-slate-300 h-10 w-full rounded-t-lg flex items-center justify-between px-4 text-slate-700 shadow-sm">
                                    <span className="text-sm font-bold uppercase">Applicants</span>
                                    <span className="font-bold text-sm">106</span>
                                </div>
                                {/* Waitlist */}
                                <div className="bg-sky-300 h-10 w-[90%] mx-auto flex items-center justify-between px-4 text-sky-900 shadow-sm">
                                    <span className="text-sm font-bold uppercase">Waitlist</span>
                                    <span className="font-bold text-sm">21</span>
                                </div>
                                {/* Processing */}
                                <div className="bg-blue-400 h-10 w-[80%] mx-auto flex items-center justify-between px-4 text-white shadow-sm">
                                    <span className="text-sm font-bold uppercase">Processing</span>
                                    <span className="font-bold text-sm">109</span>
                                </div>
                                {/* Committee */}
                                <div className="bg-indigo-500 h-10 w-[70%] mx-auto flex items-center justify-between px-4 text-white shadow-sm">
                                    <span className="text-sm font-bold uppercase">Cmte. Review</span>
                                    <span className="font-bold text-sm">84</span>
                                </div>
                                {/* Invited */}
                                <div className="bg-indigo-700 h-12 w-[60%] mx-auto rounded-b-lg flex items-center justify-between px-3 text-white shadow-md relative z-10">
                                    <span className="text-sm font-bold uppercase">Invited</span>
                                    <span className="font-bold text-lg">63</span>
                                </div>
                            </div>
                            
                            {/* Down Arrow for Funnel */}
                            <div className="h-8 w-0.5 bg-slate-300 my-1"></div>
                            
                            {/* New Members Badge */}
                            <div className="bg-emerald-100 border-2 border-emerald-500 text-emerald-800 rounded-lg px-4 py-2 flex flex-col items-center shadow-lg relative z-20">
                                <span className="text-sm font-bold uppercase">New Members (Dec)</span>
                                <span className="text-2xl font-black">27</span>
                            </div>
                        </div>

                        {/* ARROW: Funnel to Base */}
                        <div className="hidden lg:flex items-center text-slate-300">
                            <ArrowRight className="w-12 h-12" />
                        </div>
                        
                        {/* Mobile Down Arrow between Funnel and Base */}
                        <div className="flex lg:hidden items-center text-slate-300 mt-4 mb-4">
                             <ArrowDown className="w-8 h-8" />
                        </div>

                        {/* 2. MEMBERSHIP BASE (CENTER/RIGHT) - Updated to Cylinder Shape */}
                        <div className="flex flex-col items-center relative">
                            <div className="relative p-6 bg-slate-50 rounded-3xl border-4 border-double border-slate-200 w-72 h-40 flex flex-col items-center justify-center text-center shadow-inner z-20">
                                <div className="absolute top-3">
                                    <Users className="w-6 h-6 text-blue-500 opacity-50" />
                                </div>
                                <h4 className="text-base font-bold text-slate-500 uppercase tracking-wide mt-2">Membership Base</h4>
                                <div className="text-4xl font-black text-slate-800 my-1">11,588</div>
                                <div className="text-sm text-slate-400">Total Accounts</div>
                            </div>
                            
                            {/* Mobile Connector Arrow to Resigned */}
                             <div className="flex lg:hidden items-center text-slate-300 mt-4">
                                <ArrowDown className="w-8 h-8" />
                            </div>

                             {/* Resignation Exit (Bottom Right) - Responsive Positioning */}
                            <div className="static lg:absolute lg:-bottom-16 lg:-right-32 lg:top-1/2 lg:-translate-y-1/2 z-10 mt-0 lg:mt-0">
                                <div className="bg-orange-50 border border-orange-200 text-orange-700 rounded-xl p-3 shadow-md w-32 flex flex-col items-center relative">
                                    <div className="absolute top-1/2 -left-8 -translate-y-1/2 text-orange-300 hidden lg:block">
                                        <ArrowRight className="w-6 h-6" />
                                    </div>
                                    <UserMinus className="w-5 h-5 mb-1" />
                                    <span className="text-xs font-bold uppercase">Resigned</span>
                                    <span className="text-xl font-bold">40</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    {/* 3. THE REINSTATEMENT LOOP (Bottom) */}
                    <div className="mt-8 lg:mt-16 relative h-auto lg:h-24 flex justify-center"> 
                        {/* Connecting Line from Resignation back to Base/Funnel - Desktop Only */}
                        <svg className="absolute -top-4 left-1/2 -translate-x-1/2 w-[600px] h-32 pointer-events-none overflow-visible hidden lg:block">
                            <path 
                                d="M 280 10 Q 280 80, 0 80 Q -280 80, -200 40" 
                                fill="none" 
                                stroke="#a855f7" 
                                strokeWidth="3" 
                                strokeDasharray="6 4"
                                markerEnd="url(#arrowhead)"
                            />
                            <defs>
                                <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
                                <polygon points="0 0, 10 3.5, 0 7" fill="#a855f7" />
                                </marker>
                            </defs>
                        </svg>
                        
                        {/* Mobile Arrow for Reinstatement (Upward) */}
                        <div className="lg:hidden absolute -top-8 text-purple-300">
                             <ArrowRight className="w-6 h-6 -rotate-90" />
                        </div>

                        <div className="static lg:absolute lg:top-10 lg:left-1/2 lg:transform lg:-translate-x-1/2 bg-white border-2 border-purple-400 text-purple-700 rounded-full px-4 py-2 shadow-lg flex items-center gap-2 z-30">
                            <RefreshCw className="w-4 h-4" />
                            <div className="flex flex-col leading-none text-center">
                                <span className="font-bold text-sm text-purple-700">8 Reinstatements</span>
                            </div>
                        </div>
                    </div>
                </div>
            );
        };

        // NEW COMPONENT: Historical Lookback Table
        const LifecycleLookback = () => {
            const data = [
                { month: 'Jan', newApps: 52, applicants: 89, wl: 22, proc: 166, cmte: 35, invited: 77, pipeline: 372, elections: 37, base: 11769, resigned: 52, reinstate: 0 },
                { month: 'Feb', newApps: 25, applicants: 91, wl: 14, proc: 167, cmte: 56, invited: 58, pipeline: 390, elections: 28, base: 11768, resigned: 43, reinstate: 6016 },
                { month: 'Mar', newApps: 25, applicants: 98, wl: 16, proc: 115, cmte: 90, invited: 63, pipeline: 382, elections: 22, base: 11729, resigned: 55, reinstate: 4319 },
                { month: 'Apr', newApps: 25, applicants: 85, wl: 14, proc: 124, cmte: 26, invited: 113, pipeline: 362, elections: 23, base: 11722, resigned: 64, reinstate: 8738 },
                { month: 'May', newApps: 16, applicants: 107, wl: 8, proc: 86, cmte: 58, invited: 67, pipeline: 326, elections: 49, base: 11764, resigned: 68, reinstate: 1613 },
                { month: 'Jun', newApps: 54, applicants: 109, wl: 51, proc: 61, cmte: 30, invited: 107, pipeline: 358, elections: 39, base: 11751, resigned: 46, reinstate: 4116 },
                { month: 'Jul', newApps: 34, applicants: 116, wl: 25, proc: 113, cmte: 22, invited: 89, pipeline: 365, elections: 35, base: 11680, resigned: 44, reinstate: 11023 },
                { month: 'Aug', newApps: 37, applicants: 115, wl: 24, proc: 123, cmte: 26, invited: 76, pipeline: 364, elections: 18, base: 11650, resigned: 54, reinstate: 2465 },
                { month: 'Sep', newApps: 39, applicants: 114, wl: 57, proc: 105, cmte: 42, invited: 70, pipeline: 388, elections: 21, base: 11623, resigned: 64, reinstate: 6102 },
                { month: 'Oct', newApps: 38, applicants: 107, wl: 24, proc: 123, cmte: 35, invited: 70, pipeline: 359, elections: 26, base: 11602, resigned: 52, reinstate: 7092 },
                { month: 'Nov', newApps: 28, applicants: 113, wl: 18, proc: 111, cmte: 44, invited: 90, pipeline: 376, elections: 35, base: 11550, resigned: 38, reinstate: 1195 },
                { month: 'Dec', newApps: 31, applicants: 106, wl: 21, proc: 109, cmte: 84, invited: 63, pipeline: 378, elections: 27, base: 11588, resigned: 40, reinstate: 32501 },
            ];

            const totals = {
                newApps: data.reduce((a, b) => a + b.newApps, 0),
                elections: data.reduce((a, b) => a + b.elections, 0),
                resigned: data.reduce((a, b) => a + b.resigned, 0),
                reinstate: data.reduce((a, b) => a + b.reinstate, 0),
            };

            const fmt = (val) => new Intl.NumberFormat('en-US', { style: 'currency', currency: 'USD', minimumFractionDigits: 0, maximumFractionDigits: 0 }).format(val);

            // Helper for cell styling
            const Cell = ({ children, className }) => (
                <td className={`p-2 text-center text-sm text-slate-600 ${className}`}>{children}</td>
            );

            // Helper for Label styling
            const Label = ({ children, colorClass }) => (
                <td className="p-2 w-32 md:w-48 sticky left-0 bg-white z-10 border-r border-slate-100 shadow-sm">
                    <div className={`px-2 md:px-3 py-1.5 rounded-lg text-xs font-bold uppercase shadow-sm truncate ${colorClass}`}>
                        {children}
                    </div>
                </td>
            );

            // Helper for Trend Cell
            const TrendCell = ({ label, isUp, isPositive, value, type = 'flow' }) => {
                const color = isPositive ? 'text-emerald-600 bg-emerald-50' : (isPositive === false ? 'text-red-600 bg-red-50' : 'text-slate-600 bg-slate-50');
                const Icon = isUp ? TrendingUp : TrendingDown;
                return (
                    <td className="p-2 border-l border-slate-200 bg-slate-50 min-w-[80px]">
                        <div className="flex flex-col items-center">
                            <span className="font-black text-sm text-slate-800">{value}</span>
                            <span className={`flex items-center text-xs font-bold ${color} px-1.5 py-0.5 rounded-full mt-0.5`}>
                                <Icon className="w-3 h-3 mr-0.5" />
                                {type === 'flow' ? 'Total' : (isUp ? 'Up' : 'Down')}
                            </span>
                        </div>
                    </td>
                );
            };

            return (
                <div className="w-full bg-white rounded-xl border border-slate-200 shadow-sm p-4 md:p-6 mt-6 overflow-hidden">
                    <h4 className="font-bold text-slate-900 mb-4 text-lg">2025 Lifecycle Lookback</h4>
                    <div className="overflow-x-auto no-scrollbar">
                        <table className="w-full border-separate border-spacing-y-2 min-w-[800px]">
                            <thead>
                                <tr>
                                    <th className="p-2 text-left text-slate-400 font-bold text-xs uppercase tracking-wider sticky left-0 bg-white z-10 border-b border-slate-200">Metric</th>
                                    {data.map(d => <th key={d.month} className="p-2 text-slate-400 font-bold text-xs uppercase border-b border-slate-200">{d.month}</th>)}
                                    <th className="p-2 text-center text-slate-800 font-black text-xs uppercase tracking-wider bg-slate-100 rounded-t-lg border border-slate-200">Year End</th>
                                </tr>
                            </thead>
                            <tbody>
                                {/* Pipeline Section */}
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-emerald-100 text-emerald-800">New Apps</Label>
                                    {data.map((d, i) => <Cell key={i} className="font-semibold text-emerald-700">{d.newApps}</Cell>)}
                                    <TrendCell value={totals.newApps} isUp={false} isPositive={null} type="flow" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-slate-200 text-slate-700">Applicants</Label>
                                    {data.map((d, i) => <Cell key={i}>{d.applicants}</Cell>)}
                                    <TrendCell value={data[11].applicants} isUp={true} isPositive={true} type="stock" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-sky-100 text-sky-800">Waitlist</Label>
                                    {data.map((d, i) => <Cell key={i}>{d.wl}</Cell>)}
                                    <TrendCell value={data[11].wl} isUp={false} isPositive={true} type="stock" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-blue-100 text-blue-800">In Processing</Label>
                                    {data.map((d, i) => <Cell key={i}>{d.proc}</Cell>)}
                                    <TrendCell value={data[11].proc} isUp={false} isPositive={true} type="stock" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-indigo-100 text-indigo-800">Cmte. Review</Label>
                                    {data.map((d, i) => <Cell key={i}>{d.cmte}</Cell>)}
                                    <TrendCell value={data[11].cmte} isUp={true} isPositive={true} type="stock" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-indigo-200 text-indigo-900">Invited</Label>
                                    {data.map((d, i) => <Cell key={i}>{d.invited}</Cell>)}
                                    <TrendCell value={data[11].invited} isUp={false} isPositive={true} type="stock" />
                                </tr>
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <td className="p-2 text-right text-xs font-bold text-slate-400 uppercase tracking-widest pr-4 sticky left-0 bg-white z-10 border-r border-slate-100">Total Pipeline</td>
                                    {data.map((d, i) => <Cell key={i} className="font-bold text-slate-400">{d.pipeline}</Cell>)}
                                    <TrendCell value={data[11].pipeline} isUp={true} isPositive={true} type="stock" />
                                </tr>

                                {/* Base Section */}
                                <tr className="h-4"></tr> {/* Spacer */}
                                
                                <tr className="hover:bg-slate-50 transition-colors border-t border-slate-100">
                                    <Label colorClass="bg-emerald-200 text-emerald-900">Elections (In)</Label>
                                    {data.map((d, i) => <Cell key={i} className="font-bold text-emerald-700">{d.elections}</Cell>)}
                                    <TrendCell value={totals.elections} isUp={false} isPositive={null} type="flow" />
                                </tr>
                                
                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-slate-100 text-slate-800 border border-slate-200">Base Accounts</Label>
                                    {data.map((d, i) => <Cell key={i} className="font-bold text-slate-800">{d.base.toLocaleString()}</Cell>)}
                                    <TrendCell value={data[11].base.toLocaleString()} isUp={false} isPositive={false} type="stock" />
                                </tr>

                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-orange-100 text-orange-800">Resigned (Out)</Label>
                                    {data.map((d, i) => <Cell key={i} className="font-bold text-orange-700">{d.resigned}</Cell>)}
                                    <TrendCell value={totals.resigned} isUp={false} isPositive={true} type="flow" />
                                </tr>

                                {/* Loop Section */}
                                <tr className="h-4"></tr> {/* Spacer */}

                                <tr className="hover:bg-slate-50 transition-colors">
                                    <Label colorClass="bg-purple-100 text-purple-800">Reinstate Loop</Label>
                                    {data.map((d, i) => <Cell key={i} className="text-sm text-purple-700 font-medium">{fmt(d.reinstate)}</Cell>)}
                                    <TrendCell value={fmt(totals.reinstate)} isUp={true} isPositive={true} type="flow" />
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            )
        }

        // REMOVED Member Type Breakdown Table

        const MembershipDashboard = () => {
            // December Data (Updated from Nov)
            const fluxData = [
                { name: 'Headcount', New: 86, Resigned: 50, Net: 36 },
                { name: 'Accounts', New: 27, Resigned: 40, Net: -13 }
            ];

            // Membership Flux YTD 2025 Data
            const fluxYTDData = [
                { month: 'Jan', AccNew: 37, AccRes: 52, HeadNew: 74, HeadRes: 63 },
                { month: 'Feb', AccNew: 28, AccRes: 43, HeadNew: 92, HeadRes: 62 },
                { month: 'Mar', AccNew: 22, AccRes: 55, HeadNew: 50, HeadRes: 66 },
                { month: 'Apr', AccNew: 23, AccRes: 64, HeadNew: 60, HeadRes: 89 },
                { month: 'May', AccNew: 49, AccRes: 68, HeadNew: 109, HeadRes: 101 },
                { month: 'Jun', AccNew: 39, AccRes: 46, HeadNew: 122, HeadRes: 64 },
                { month: 'Jul', AccNew: 35, AccRes: 44, HeadNew: 87, HeadRes: 76 },
                { month: 'Aug', AccNew: 18, AccRes: 54, HeadNew: 69, HeadRes: 91 },
                { month: 'Sep', AccNew: 21, AccRes: 64, HeadNew: 58, HeadRes: 91 },
                { month: 'Oct', AccNew: 26, AccRes: 52, HeadNew: 40, HeadRes: 78 },
                { month: 'Nov', AccNew: 35, AccRes: 38, HeadNew: 61, HeadRes: 53 },
                { month: 'Dec', AccNew: 27, AccRes: 40, HeadNew: 86, HeadRes: 50 },
            ];

            // Updated Pipeline Data for November
            const pipelineData = [
                { name: 'Applicants', value: 106, fill: '#94a3b8', desc: 'Has completed an application AND has paid application fee $100' },
                { name: 'Deposits/WL', fullName: 'Waitlist', value: 21, fill: '#60a5fa', desc: 'Has submitted deposit or is legacy and or spouse internal waitlist' },
                { name: 'In Processing', value: 109, fill: '#3b82f6', desc: 'Pulled off waitlist to begin pre-governance review, required 30-day posting, background checks, confirm letters of recommendation' },
                { name: 'Cmte. Review', fullName: 'Committee Review', value: 84, fill: '#2563eb', desc: 'Application package is submitted and under Membership Committee and/or Board Review' },
                { name: 'Invited', value: 63, fill: '#1d4ed8', desc: 'Formally invited to join' }
            ];

            // Consolidated Financial Data (Dec 2025 & YTD)
            const combinedPipelineFinancials = [
                {
                    title: "New Deposits",
                    icon: Wallet,
                    color: "text-emerald-600",
                    bg: "bg-emerald-100",
                    dec: { value: 97600, label: "22 Accounts", trend: "Up 46% MoM", trendUp: true },
                    ytd: { value: 896150, trend: "40% YoY", trendUp: true }
                },
                {
                    title: "Remaining Election Checks",
                    icon: DollarSign,
                    color: "text-blue-600",
                    bg: "bg-blue-100",
                    dec: { value: 100584, label: "16 Checks", trend: "Down -34% MoM", trendUp: false },
                    ytd: { value: "$1.21m", trend: "60% YoY", trendUp: true } // Value is string here
                },
                {
                    title: "Application Fees",
                    icon: FileText,
                    color: "text-indigo-600",
                    bg: "bg-indigo-100",
                    dec: { value: 1600, label: "16 Apps", trend: "Same MoM", trendNeutral: true },
                    ytd: { value: 23000, trend: "10% YoY", trendUp: false } 
                },
                {
                    title: "Reinstatements",
                    icon: Activity,
                    color: "text-purple-600",
                    bg: "bg-purple-100",
                    dec: { value: 32501, label: "8 Reinstatements", trend: "Up 95% MoM", trendUp: true },
                    ytd: { value: 85178, trend: "", trendNeutral: true }
                }
            ];

            // YTD Metrics - UPDATED with Descriptions, Exception Requests Removed
            const ytdMetrics = [
                { 
                    label: 'Applications Reviewed', 
                    value: 380, 
                    icon: ClipboardList, 
                    color: 'text-blue-600', 
                    bg: 'bg-blue-50', 
                    trend: '6% YoY', 
                    trendColor: 'text-emerald-600', 
                    trendBg: 'bg-emerald-50', 
                    TrendIcon: TrendingUp,
                    desc: "Number of Applications in 2025 put forth for the Membership Committee's review for recommendation."
                },
                { 
                    label: 'New Members Onboarded', 
                    value: 358, 
                    icon: UserPlus, 
                    color: 'text-emerald-600', 
                    bg: 'bg-emerald-50', 
                    trend: '18% YoY', 
                    trendColor: 'text-emerald-600', 
                    trendBg: 'bg-emerald-50', 
                    TrendIcon: TrendingUp,
                    desc: "Number of New Elected Members who have accepted their invitation to membership and solidified their initiation fee."
                },
                { 
                    label: 'Total Resignations', 
                    value: 620, 
                    icon: UserMinus, 
                    color: 'text-orange-600', 
                    bg: 'bg-orange-50', 
                    trend: '10% YoY', 
                    trendColor: 'text-red-600', 
                    trendBg: 'bg-red-50', 
                    TrendIcon: TrendingUp,
                    desc: "Number of adult members who have submitted a request for resign."
                },
                { 
                    label: 'Accounts in Pipeline', 
                    value: 383, 
                    icon: Database, 
                    color: 'text-violet-600', 
                    bg: 'bg-violet-50', 
                    trend: '3%', 
                    trendColor: 'text-red-600', 
                    trendBg: 'bg-red-50', 
                    TrendIcon: TrendingDown,
                    desc: "Number of account records in the process of applying for membership."
                },
                { 
                    label: 'Intermediates Elected', 
                    value: 102, 
                    icon: CheckCircle, 
                    color: 'text-indigo-600', 
                    bg: 'bg-indigo-50', 
                    trend: '38% YoY', 
                    trendColor: 'text-emerald-600', 
                    trendBg: 'bg-emerald-50', 
                    TrendIcon: TrendingUp,
                    desc: "Number of Intermediate Members in 2025 who accepted their invitation to membership and solidified their initiation fee."
                },
                { 
                    label: 'Juniors Transferred to Intermediate', 
                    value: 308, 
                    icon: UserCheck, 
                    color: 'text-cyan-600', 
                    bg: 'bg-cyan-50', 
                    trend: '18% YoY', 
                    trendColor: 'text-emerald-600', 
                    trendBg: 'bg-emerald-50', 
                    TrendIcon: TrendingUp,
                    desc: "Number of junior members who have turned 18 and completed a junior to intermediate transfer form and are paying intermediate dues."
                },
            ];

            const newAccountsBreakdown = [
                { label: 'Family', count: 8, amount: 3378.72 },
                { label: 'Individual Under 30', count: 6, amount: 323.64 },
                { label: 'Individual', count: 5, amount: 1400.55 },
                { label: 'Spouse', count: 4, amount: 568.92 },
                { label: 'Family of 2', count: 1, amount: 400.11 },
                { label: 'Nonresident Family 30-34', count: 1, amount: 98.01 },
                { label: 'Nonresident Family Under 30', count: 1, amount: 79.14 },
                { label: 'Nonresident Under 30', count: 1, amount: 79.14 },
                { label: 'Juniors to Intermediate (+41)', count: '', amount: 1367.25, highlight: true }
            ];

            const resignedAccountsBreakdown = [
                { label: 'Intermediate', count: 12, amount: 400.20 },
                { label: 'Individual', count: 6, amount: 1680.66 },
                { label: 'Individual Preferred Tier 3', count: 3, amount: 560.04 },
                { label: 'Family', count: 2, amount: 844.68 },
                { label: 'Family of 2', count: 2, amount: 800.22 },
                { label: 'Nonresident', count: 2, amount: 224.12 },
                { label: 'Nonresident 30-34', count: 2, amount: 196.02 },
                { label: 'Nonresident Family of 2', count: 2, amount: 320.14 },
                { label: 'Adult Athletic Family', count: 1, amount: 280.11 },
                { label: 'Family Preferred Tier 2', count: 1, amount: 297.84 },
                { label: 'Family Preferred Tier 3', count: 1, amount: 266.72 },
                { label: 'Individual Preferred Tier 2', count: 1, amount: 208.46 },
                { label: 'Individual Preferred Tier 4', count: 1, amount: 124.50 },
                { label: 'Nonresident Family', count: 1, amount: 168.96 },
                { label: 'Nonresident Spouse', count: 1, amount: 56.90 },
                { label: 'Spouse', count: 1, amount: 142.23 },
                { label: 'Spouse Preferred', count: 1, amount: 100.08 },
            ];

            // 2025 History Data
            const pipelineHistoryData = [
                { month: 'Jan', Applicants: 89, Waitlist: 22, Processing: 166, Committee: 35, Invited: 77 },
                { month: 'Feb', Applicants: 91, Waitlist: 14, Processing: 167, Committee: 56, Invited: 58 },
                { month: 'Mar', Applicants: 98, Waitlist: 16, Processing: 115, Committee: 90, Invited: 63 },
                { month: 'Apr', Applicants: 85, Waitlist: 14, Processing: 124, Committee: 26, Invited: 113 },
                { month: 'May', Applicants: 107, Waitlist: 8, Processing: 86, Committee: 58, Invited: 67 },
                { month: 'Jun', Applicants: 109, Waitlist: 51, Processing: 61, Committee: 30, Invited: 107 },
                { month: 'Jul', Applicants: 116, Waitlist: 25, Processing: 113, Committee: 22, Invited: 89 },
                { month: 'Aug', Applicants: 115, Waitlist: 24, Processing: 123, Committee: 26, Invited: 76 },
                { month: 'Sep', Applicants: 114, Waitlist: 57, Processing: 105, Committee: 42, Invited: 70 },
                { month: 'Oct', Applicants: 107, Waitlist: 24, Processing: 123, Committee: 35, Invited: 70 },
                { month: 'Nov', Applicants: 113, Waitlist: 18, Processing: 111, Committee: 44, Invited: 90 },
                { month: 'Dec', Applicants: 106, Waitlist: 21, Processing: 109, Committee: 84, Invited: 63 },
            ];

            const cashEconomicsData = [
                { month: 'Jan', AppFees: 2100, Deposits: 61200, Capital: 36000, Total: 99300 },
                { month: 'Feb', AppFees: 1400, Deposits: 65000, Capital: 102500, Total: 168900 },
                { month: 'Mar', AppFees: 1600, Deposits: 70600, Capital: 43000, Total: 115200 },
                { month: 'Apr', AppFees: 1500, Deposits: 52000, Capital: 105000, Total: 158500 },
                { month: 'May', AppFees: 1300, Deposits: 83300, Capital: 226250, Total: 310850 },
                { month: 'Jun', AppFees: 1700, Deposits: 74600, Capital: 131100, Total: 207400 },
                { month: 'Jul', AppFees: 2200, Deposits: 69700, Capital: 112296, Total: 184196 },
                { month: 'Aug', AppFees: 1400, Deposits: 83650, Capital: 85000, Total: 170050 },
                { month: 'Sep', AppFees: 2400, Deposits: 90200, Capital: 59000, Total: 151600 },
                { month: 'Oct', AppFees: 1700, Deposits: 96000, Capital: 77700, Total: 175400 },
                { month: 'Nov', AppFees: 1600, Deposits: 52300, Capital: 134596, Total: 188496 },
                { month: 'Dec', AppFees: 1600, Deposits: 97600, Capital: 100584, Total: 232285 },
            ];

            const formatCurrency = (val) => new Intl.NumberFormat('en-US', { style: 'currency', currency: 'USD', maximumFractionDigits: 0 }).format(val);
            const formatCurrencyPrecise = (val) => new Intl.NumberFormat('en-US', { style: 'currency', currency: 'USD', minimumFractionDigits: 2 }).format(val);

            // Custom Tooltip for Pipeline to show descriptions
            const CustomPipelineTooltip = ({ active, payload }) => {
                if (active && payload && payload.length) {
                    const data = payload[0].payload;
                    return (
                        <div className="bg-white p-3 border border-slate-200 shadow-xl rounded-lg max-w-xs z-50">
                            <p className="font-bold text-slate-900">{data.fullName || data.name}</p>
                            <p className="text-xl font-bold text-blue-600 my-1">{data.value}</p>
                            <p className="text-xs text-slate-500 leading-snug">{data.desc}</p>
                        </div>
                    );
                }
                return null;
            };

            // --- EXAMPLE CENSUS DATA ---
            const censusAgeData = [
                { name: '< 18', value: 4359, fill: '#cbd5e1' },
                { name: '18-29', value: 2180, fill: '#94a3b8' },
                { name: '30-49', value: 7629, fill: '#64748b' },
                { name: '50-69', value: 5450, fill: '#475569' },
                { name: '70+', value: 2181, fill: '#334155' },
            ];

            const censusTypeData = [
                { name: 'Family', value: 8720, fill: '#3b82f6' },
                { name: 'Individual', value: 6540, fill: '#10b981' },
                { name: 'Junior', value: 3270, fill: '#f59e0b' },
                { name: 'Nonresident', value: 2180, fill: '#6366f1' },
                { name: 'Other', value: 1089, fill: '#94a3b8' },
            ];

            // Custom Legend Payload to enforce correct label order (Applicants -> Invited)
            const pipelineLegend = [
                { value: 'Applicants', type: 'rect', color: '#94a3b8', id: 'Applicants' },
                { value: 'Waitlist', type: 'rect', color: '#60a5fa', id: 'Waitlist' },
                { value: 'In Processing', type: 'rect', color: '#3b82f6', id: 'Processing' },
                { value: 'Cmte. Review', type: 'rect', color: '#2563eb', id: 'Committee' },
                { value: 'Invited', type: 'rect', color: '#1d4ed8', id: 'Invited' }
            ];

            return (
                <div className="min-h-screen bg-slate-50 p-4 md:p-8 font-sans text-slate-900">
                    {/* Header */}
                    <header className="mb-8 border-b border-slate-200 pb-6">
                        <div className="flex flex-col md:flex-row md:items-start justify-between gap-6">
                            <div className="max-w-2xl">
                                <h1 className="text-4xl font-extrabold text-slate-900 tracking-tight">Membership Dashboard</h1>
                                <p className="text-slate-500 mt-2 text-lg">2025 Performance Overview</p>
                            </div>
                            <div className="mt-6 md:mt-0 flex flex-col sm:flex-row flex-wrap gap-4 justify-end">
                                <div className="px-6 py-4 bg-white rounded-xl border border-slate-200 shadow-sm text-center w-full sm:w-auto">
                                    <span className="text-sm font-bold text-slate-400 uppercase tracking-widest block mb-1">Total Members</span>
                                    <div className="flex items-baseline justify-center gap-2">
                                        <span className="text-3xl font-black text-slate-800">21,837</span>
                                        <div className="flex flex-col gap-1 items-start">
                                            <span className="flex items-center text-[10px] font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded-full">
                                                <TrendingUp className="w-3 h-3 mr-1" />
                                                +0.17% MoM
                                            </span>
                                            <span className="flex items-center text-[10px] font-bold text-red-600 bg-red-50 px-2 py-0.5 rounded-full">
                                                <TrendingDown className="w-3 h-3 mr-1" />
                                                -1.62% YoY
                                            </span>
                                        </div>
                                    </div>
                                    <p className="text-xs text-slate-400 mt-2 max-w-[150px] mx-auto leading-tight">Total number of active child, junior, intermediate or adult members</p>
                                </div>
                                <div className="px-6 py-4 bg-white rounded-xl border border-slate-200 shadow-sm text-center w-full sm:w-auto">
                                    <span className="text-sm font-bold text-slate-400 uppercase tracking-widest block mb-1">Total Accounts</span>
                                    <div className="flex items-baseline justify-center gap-2">
                                        <span className="text-3xl font-black text-slate-800">11,588</span>
                                        <div className="flex flex-col gap-1 items-start">
                                            <span className="flex items-center text-[10px] font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded-full">
                                                <TrendingUp className="w-3 h-3 mr-1" />
                                                +1.86% MoM
                                            </span>
                                            <span className="flex items-center text-[10px] font-bold text-red-600 bg-red-50 px-2 py-0.5 rounded-full">
                                                <TrendingDown className="w-3 h-3 mr-1" />
                                                -2.79% YoY
                                            </span>
                                        </div>
                                    </div>
                                    <p className="text-xs text-slate-400 mt-2 max-w-[150px] mx-auto leading-tight">An account = one membership. One family, one couple, or one individual.</p>
                                </div>
                                <div className="px-6 py-4 bg-white rounded-xl border border-slate-200 shadow-sm text-center w-full sm:w-auto">
                                    <span className="text-sm font-bold text-slate-400 uppercase tracking-widest block mb-1">Dues Revenue</span>
                                    <div className="flex items-baseline justify-center gap-2">
                                        <span className="text-3xl font-black text-slate-800">$35.28M</span>
                                        <span className="flex items-center text-xs font-bold text-emerald-600 bg-emerald-50 px-1.5 py-0.5 rounded-full">
                                            <CheckCircle className="w-3 h-3 mr-0.5" />
                                            On Target
                                        </span>
                                    </div>
                                </div>
                                {/* Avg Monthly Elections */}
                                <div className="px-6 py-4 bg-white rounded-xl border border-slate-200 shadow-sm text-center w-full sm:w-auto">
                                    <span className="text-sm font-bold text-slate-400 uppercase tracking-widest block mb-1">Average Monthly Elections 2025</span>
                                    <div className="flex items-baseline justify-center gap-2">
                                        <span className="text-3xl font-black text-slate-800">30</span>
                                        <span className="flex items-center text-xs font-bold text-emerald-600 bg-emerald-50 px-1.5 py-0.5 rounded-full">
                                            <TrendingUp className="w-3 h-3 mr-0.5" />
                                            20% YoY
                                        </span>
                                    </div>
                                </div>
                                {/* Avg Monthly Resignations */}
                                <div className="px-6 py-4 bg-white rounded-xl border border-slate-200 shadow-sm text-center w-full sm:w-auto">
                                    <span className="text-sm font-bold text-slate-400 uppercase tracking-widest block mb-1">Average Monthly Resignations 2025</span>
                                    <div className="flex items-baseline justify-center gap-2">
                                        <span className="text-3xl font-black text-slate-800">52</span>
                                        <span className="flex items-center text-xs font-bold text-red-600 bg-red-50 px-1.5 py-0.5 rounded-full">
                                            <TrendingUp className="w-3 h-3 mr-0.5" />
                                            10% YoY
                                        </span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </header>

                    {/* YTD Snapshot Section */}
                    <div className="mb-10">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-slate-800 w-2 h-6 mr-3 rounded-sm"></span>
                            Membership Snapshot (YTD 2025)
                        </h2>
                        {/* Adjusted grid for new item */}
                        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6"> 
                            {ytdMetrics.map((metric, idx) => {
                                const TrendIconComponent = metric.TrendIcon || TrendingUp;
                                return (
                                    <div key={idx} className="bg-white p-5 rounded-xl border border-slate-200 shadow-sm flex flex-col justify-start h-full hover:shadow-md transition-shadow">
                                        <div className="flex justify-between items-start mb-4">
                                            <div className={`p-2.5 rounded-lg ${metric.bg}`}>
                                                <metric.icon className={`w-5 h-5 ${metric.color}`} />
                                            </div>
                                            {metric.trend && (
                                                <span className={`flex items-center text-xs font-bold ${metric.trendColor || 'text-emerald-600'} ${metric.trendBg || 'bg-emerald-50'} px-2 py-0.5 rounded-full whitespace-nowrap`}>
                                                    <TrendIconComponent className="w-3 h-3 mr-1" />
                                                    {metric.trend}
                                                </span>
                                            )}
                                        </div>
                                        <div>
                                            <div className="text-3xl font-black text-slate-900 mb-1">{metric.value}</div>
                                            <div className="text-sm font-bold text-slate-700 mb-2">{metric.label}</div>
                                            <p className="text-sm text-slate-500 leading-relaxed">{metric.desc}</p>
                                        </div>
                                    </div>
                                );
                            })}
                        </div>
                    </div>

                    {/* Top Level Monthly KPIs */}
                    <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                        <span className="bg-blue-600 w-2 h-6 mr-3 rounded-sm"></span>
                        December Monthly Performance
                    </h2>
                    
                    {/* Primary KPIs */}
                    <div className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
                        {/* Net Monthly Dues Change */}
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                            <div className="flex items-center justify-between mb-4">
                                <h3 className="text-sm font-semibold text-slate-500">December 2025 Net Dues Change</h3>
                                <div className="p-2 bg-emerald-50 rounded-lg">
                                    <TrendingUp className="w-5 h-5 text-emerald-600" />
                                </div>
                            </div>
                            <div className="flex items-baseline gap-2 mb-1">
                                <div className="text-2xl font-bold text-emerald-600">+$1,023.60</div>
                                <span className="flex items-center text-xs font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded-full">
                                    <TrendingUp className="w-3 h-3 mr-1" />
                                    New Adds {'>'} Resignations
                                </span>
                            </div>
                        </div>

                        {/* New Accounts Value */}
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                            <div className="flex items-center justify-between mb-4">
                                <h3 className="text-sm font-semibold text-slate-500">December 2025 New Accounts Value</h3>
                                <div className="p-2 bg-emerald-50 rounded-lg">
                                    <UserPlus className="w-5 h-5 text-emerald-600" />
                                </div>
                            </div>
                            <div className="flex items-baseline gap-2 mb-1">
                                <div className="text-2xl font-bold text-emerald-600">+$7,695.58</div>
                                <p className="text-sm text-slate-400">From 27 new accounts</p>
                            </div>
                        </div>

                        {/* Resigned Value */}
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                            <div className="flex items-center justify-between mb-4">
                                <h3 className="text-sm font-semibold text-slate-500">December 2025 Resigned Accounts Value</h3>
                                <div className="p-2 bg-orange-50 rounded-lg">
                                    <UserMinus className="w-5 h-5 text-orange-600" />
                                </div>
                            </div>
                            <div className="flex items-baseline gap-2 mb-1">
                                <div className="text-2xl font-bold text-orange-600">-$6,671.88</div>
                                <p className="text-sm text-slate-400">From 40 resigned accounts</p>
                            </div>
                        </div>
                    </div>

                    {/* Breakdown Details Row */}
                    <div className="grid grid-cols-1 lg:grid-cols-2 gap-6 mb-8">
                        {/* New Accounts Breakdown */}
                        <div className="bg-white p-5 rounded-xl border border-slate-200 shadow-sm h-full">
                            <div className="flex items-center justify-between mb-4 pb-2 border-b border-slate-100">
                                <div>
                                    <h3 className="font-bold text-slate-900">New Accounts By Type (December 2025)</h3>
                                    <p className="text-sm text-slate-500 mt-1">New elected accounts and juniors that transferred to Intermediate</p>
                                </div>
                                <span className="px-2 py-1 bg-emerald-100 text-emerald-800 text-xs font-bold rounded-full">27 Total</span>
                            </div>
                            <div className="space-y-3">
                                {newAccountsBreakdown.map((item, idx) => (
                                    <div key={idx} className={`flex justify-between items-center text-sm ${item.highlight ? 'pt-2 mt-2 border-t border-slate-100 font-semibold' : ''}`}>
                                        <span className={`text-slate-600 ${item.highlight ? 'text-emerald-700' : ''}`}>{item.label}</span>
                                        <div className="flex gap-4">
                                            <span className="font-bold text-slate-900 w-6 text-right">{item.count}</span>
                                            <span className="font-bold text-slate-600 w-20 text-right">{formatCurrencyPrecise(item.amount)}</span>
                                        </div>
                                    </div>
                                ))}
                                <div className="flex justify-between items-center text-sm pt-2 mt-2 border-t-2 border-slate-100">
                                    <span className="font-bold text-slate-800">Total</span>
                                    <span className="font-black text-emerald-600">$7,695.48</span>
                                </div>
                            </div>
                        </div>

                        {/* Resigned Accounts Breakdown */}
                        <div className="bg-white p-5 rounded-xl border border-slate-200 shadow-sm h-full">
                            <div className="flex items-center justify-between mb-4 pb-2 border-b border-slate-100">
                                <div>
                                    <h3 className="font-bold text-slate-900">Resignations by Type</h3>
                                    <p className="text-sm text-slate-500 mt-1">Number of accounts that resigned in December 2025</p>
                                </div>
                                <span className="px-2 py-1 bg-orange-100 text-orange-800 text-xs font-bold rounded-full">40 Total</span>
                            </div>
                            <div className="space-y-2">
                                <div className="flex justify-between text-xs font-bold text-slate-400 uppercase mb-2">
                                    <span>Membership Type</span>
                                    <div className="flex gap-4">
                                        <span className="w-6 text-right">Count</span>
                                        <span className="w-20 text-right">Dues Impact</span>
                                    </div>
                                </div>
                                {resignedAccountsBreakdown.map((item, idx) => (
                                    <div key={idx} className="flex justify-between items-center text-sm">
                                        <span className="text-slate-600">{item.label}</span>
                                        <div className="flex gap-4">
                                            <span className="font-bold text-slate-900 w-6 text-right">{item.count}</span>
                                            <span className="font-bold text-slate-600 w-20 text-right">{formatCurrencyPrecise(item.amount)}</span>
                                        </div>
                                    </div>
                                ))}
                                <div className="flex justify-between items-center text-sm pt-2 mt-2 border-t-2 border-slate-100">
                                    <span className="font-bold text-slate-800">Total</span>
                                    <div className="flex gap-4">
                                        <span className="font-black text-slate-800 w-6 text-right">40</span>
                                        <span className="font-black text-orange-600 w-20 text-right">-$6,671.88</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    {/* Charts Section */}
                    <div className="grid grid-cols-1 xl:grid-cols-2 gap-8 mb-10">
                        
                        {/* Membership Flux Chart */}
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm flex flex-col">
                            <div className="mb-4">
                                <h3 className="text-lg font-bold text-slate-900">Membership Changes (Dec)</h3>
                                <p className="text-sm text-slate-500">Comparison of Number of Accounts and Headcount Changes in December 2025</p>
                            </div>
                            <div className="h-64 w-full"> 
                                <ResponsiveContainer width="100%" height="100%">
                                    <BarChart
                                        data={fluxData}
                                        margin={{ top: 20, right: 30, left: 0, bottom: 5 }}
                                    >
                                        <CartesianGrid strokeDasharray="3 3" vertical={false} stroke="#e2e8f0" />
                                        <XAxis dataKey="name" axisLine={false} tickLine={false} tick={{fill: '#64748b', fontSize: 12}} dy={10} />
                                        <YAxis axisLine={false} tickLine={false} tick={{fill: '#64748b', fontSize: 12}} />
                                        <Tooltip 
                                            cursor={{fill: '#f1f5f9'}}
                                            contentStyle={{borderRadius: '8px', border: 'none', boxShadow: '0 4px 6px -1px rgb(0 0 0 / 0.1)'}}
                                        />
                                        <Legend iconType="circle" wrapperStyle={{paddingTop: '20px'}} />
                                        <ReferenceLine y={0} stroke="#94a3b8" />
                                        <Bar dataKey="New" fill="#10b981" name="New (Inflow)" radius={[4, 4, 0, 0]} barSize={48} />
                                        <Bar dataKey="Resigned" fill="#ef4444" name="Resigned (Outflow)" radius={[4, 4, 0, 0]} barSize={48} />
                                    </BarChart>
                                </ResponsiveContainer>
                            </div>
                        </div>

                        {/* Membership Pipeline Funnel - RESTORED HERE */}
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm flex flex-col">
                            {/* Header Area with new small tile */}
                            <div className="mb-6 flex flex-col sm:flex-row sm:items-start justify-between gap-4">
                                <div>
                                    <h3 className="text-lg font-bold text-slate-900">Membership Pipeline</h3>
                                    <p className="text-sm text-slate-500">Current Candidate Status</p>
                                    <p className="text-sm text-slate-500 mt-2 max-w-xs leading-relaxed">The pipeline evolved to remain flexible while preserving governance. There are 5 pathways to membership (Waitlist, Legacy, Spouse, Diversity Admissions and Athletic). Although there are varying pathways for admissions, every applicant moves through the same governance-controlled admissions pipeline.</p>
                                </div>
                                {/* New Small Tile Next to Pipeline */}
                                <div className="flex items-center px-4 py-2 bg-blue-50 rounded-lg border border-blue-100 shadow-sm">
                                    <Layers className="w-5 h-5 text-blue-600 mr-3" />
                                    <div>
                                        <span className="block text-xs font-bold text-blue-500 uppercase tracking-wider">Total Accounts</span>
                                        <span className="text-lg font-bold text-blue-900 leading-none">383</span>
                                    </div>
                                </div>
                            </div>
                            
                            <div className="flex-grow flex flex-col md:flex-row gap-6">
                                <div className="h-[300px] w-full md:w-1/2">
                                    <ResponsiveContainer width="100%" height="100%">
                                        <BarChart
                                            layout="vertical"
                                            data={pipelineData}
                                            margin={{ top: 0, right: 30, left: 40, bottom: 0 }}
                                        >
                                            <CartesianGrid strokeDasharray="3 3" horizontal={false} stroke="#e2e8f0" />
                                            <XAxis type="number" hide />
                                            <YAxis 
                                                dataKey="name" 
                                                type="category" 
                                                width={90} 
                                                tick={{fill: '#475569', fontSize: 11, fontWeight: 600}} 
                                                axisLine={false} 
                                                tickLine={false} 
                                            />
                                            <Tooltip content={<CustomPipelineTooltip />} cursor={{fill: '#f8fafc'}} />
                                            <Bar dataKey="value" radius={[0, 4, 4, 0]} barSize={32}>
                                                {pipelineData.map((entry, index) => (
                                                    <Cell key={`cell-${index}`} fill={entry.fill} />
                                                ))}
                                                <LabelList dataKey="value" position="right" style={{fill: '#334155', fontSize: 12, fontWeight: 'bold'}} />
                                            </Bar>
                                        </BarChart>
                                    </ResponsiveContainer>
                                </div>

                                <div className="w-full md:w-1/2 flex flex-col justify-center space-y-4 pr-2">
                                    {pipelineData.map((item, idx) => (
                                        <div key={idx} className="flex flex-col border-l-[3px] pl-3 py-1" style={{borderColor: item.fill}}>
                                            <div className="flex items-baseline justify-between">
                                                <span className="text-xs font-bold text-slate-700 uppercase tracking-wide">{item.fullName || item.name}</span>
                                            </div>
                                            <p className="text-sm text-slate-500 leading-relaxed mt-1">{item.desc}</p>
                                        </div>
                                    ))}
                                </div>
                            </div>
                        </div>
                    </div>

                    {/* Pipeline Payments December 2025 - Moved Here */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-emerald-600 w-2 h-6 mr-3 rounded-sm"></span>
                            MAC Pipeline Investments Dec 2025 & YTD
                        </h2>
                        <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
                            {combinedPipelineFinancials.map((item, index) => {
                                const DecTrendIcon = item.dec.trendNeutral ? null : (item.dec.trendUp ? TrendingUp : TrendingDown);
                                const YTDTrendIcon = item.ytd.trendNeutral ? null : (item.ytd.trendUp ? TrendingUp : TrendingDown);

                                return (
                                    <div key={index} className="bg-white p-5 rounded-xl border border-slate-200 shadow-sm flex flex-col h-full">
                                        <div className="flex items-center mb-4">
                                            <div className={`p-2 rounded-full ${item.bg} mr-3`}>
                                                <item.icon className={`w-5 h-5 ${item.color}`} />
                                            </div>
                                            <h4 className="font-bold text-slate-700 text-sm">{item.title}</h4>
                                        </div>
                                        
                                        {/* December Section */}
                                        <div className="mb-4 pb-4 border-b border-slate-100">
                                            <div className="text-sm font-bold text-slate-400 uppercase tracking-wide mb-1">December 2025</div>
                                            <div className="flex flex-col gap-1">
                                                <div className="flex items-baseline gap-2">
                                                    <span className="text-2xl font-black text-slate-900">{typeof item.dec.value === 'number' ? formatCurrency(item.dec.value) : item.dec.value}</span>
                                                    {item.dec.trend && (
                                                        <span className={`flex items-center text-xs font-bold px-1.5 py-0.5 rounded-full ${item.dec.trendNeutral ? 'bg-slate-100 text-slate-600' : (item.dec.trendUp ? 'bg-emerald-50 text-emerald-600' : 'bg-red-50 text-red-600')}`}>
                                                            {DecTrendIcon && <DecTrendIcon className="w-3 h-3 mr-0.5" />}
                                                            {item.dec.trend}
                                                        </span>
                                                    )}
                                                </div>
                                                <span className="text-sm font-medium text-slate-500">{item.dec.label}</span>
                                            </div>
                                        </div>

                                        {/* YTD Section */}
                                        <div>
                                            <div className="text-sm font-bold text-slate-400 uppercase tracking-wide mb-1">YTD 2025</div>
                                            <div className="flex items-baseline gap-2">
                                                <span className="text-xl font-bold text-slate-800">{typeof item.ytd.value === 'number' ? formatCurrency(item.ytd.value) : item.ytd.value}</span>
                                                {item.ytd.trend && (
                                                    <span className={`flex items-center text-xs font-bold px-1.5 py-0.5 rounded-full ${item.ytd.trendNeutral ? 'bg-slate-100 text-slate-600' : (item.ytd.trendUp ? 'bg-emerald-50 text-emerald-600' : 'bg-red-50 text-red-600')}`}>
                                                        {YTDTrendIcon && <YTDTrendIcon className="w-3 h-3 mr-0.5" />}
                                                        {item.ytd.trend}
                                                    </span>
                                                )}
                                            </div>
                                        </div>
                                    </div>
                                );
                            })}
                        </div>
                    </div>

                    {/* NEW SECTION: Membership Changes YTD 2025 */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-2 flex items-center">
                            <span className="bg-slate-800 w-2 h-6 mr-3 rounded-sm"></span>
                            Membership Changes YTD 2025
                        </h2>
                        <div className="mb-6 text-sm text-slate-500 max-w-4xl leading-relaxed">
                            <p className="mb-1">Membership health is determined by lifecycle balance — not by any single entry or exit signal.</p>
                            <p className="mb-1">Membership volume reflects flow, not a static count. Month-to-month change is expected and governed.</p>
                            <p>No single metric (pipeline, resignations, or elections) explains system health.</p>
                        </div>

                        <div className="grid grid-cols-1 lg:grid-cols-2 gap-8">
                            {/* Accounts YTD */}
                            <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                                <div className="mb-4">
                                    <h3 className="font-bold text-slate-900 text-lg">Account: Adds vs. Drops</h3>
                                    <p className="text-sm text-slate-500 mt-1 leading-snug">Total number of membership accounts added and resigned. This only includes adult new elections and adult resignation accounts resigned. Does not include deactivated children or juniors, suspensions, temporary members or deceased.</p>
                                </div>
                                <div className="h-64 w-full">
                                    <ResponsiveContainer width="100%" height="100%">
                                        <BarChart
                                            data={fluxYTDData}
                                            margin={{ top: 20, right: 30, left: 0, bottom: 5 }}
                                        >
                                            <CartesianGrid strokeDasharray="3 3" vertical={false} />
                                            <XAxis dataKey="month" tick={{fill: '#64748b', fontSize: 12}} />
                                            <YAxis tick={{fill: '#64748b', fontSize: 12}} />
                                            <Tooltip contentStyle={{borderRadius: '8px', border: 'none', boxShadow: '0 4px 6px -1px rgb(0 0 0 / 0.1)'}} />
                                            <Legend wrapperStyle={{paddingTop: '10px'}}/>
                                            <Bar dataKey="AccNew" fill="#10b981" name="New (Inflow)" radius={[4, 4, 0, 0]} />
                                            <Bar dataKey="AccRes" fill="#ef4444" fillOpacity={0.6} name="Resigned (Outflow)" radius={[4, 4, 0, 0]} />
                                        </BarChart>
                                    </ResponsiveContainer>
                                </div>
                            </div>

                            {/* Headcount YTD */}
                            <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                                <div className="mb-4">
                                    <h3 className="font-bold text-slate-900 text-lg">Headcount: Adds vs. Drops</h3>
                                    <p className="text-sm text-slate-500 mt-1 leading-snug">Total number of members added and dropped. This includes all membership types. This includes any age and membership type that are net "new" to the system.</p>
                                </div>
                                <div className="h-64 w-full">
                                    <ResponsiveContainer width="100%" height="100%">
                                        <BarChart
                                            data={fluxYTDData}
                                            margin={{ top: 20, right: 30, left: 0, bottom: 5 }}
                                        >
                                            <CartesianGrid strokeDasharray="3 3" vertical={false} />
                                            <XAxis dataKey="month" tick={{fill: '#64748b', fontSize: 12}} />
                                            <YAxis tick={{fill: '#64748b', fontSize: 12}} />
                                            <Tooltip contentStyle={{borderRadius: '8px', border: 'none', boxShadow: '0 4px 6px -1px rgb(0 0 0 / 0.1)'}} />
                                            <Legend wrapperStyle={{paddingTop: '10px'}}/>
                                            <Bar dataKey="HeadNew" fill="#10b981" name="New (Inflow)" radius={[4, 4, 0, 0]} />
                                            <Bar dataKey="HeadRes" fill="#ef4444" fillOpacity={0.6} name="Resigned (Outflow)" radius={[4, 4, 0, 0]} />
                                        </BarChart>
                                    </ResponsiveContainer>
                                </div>
                            </div>
                        </div>
                    </div>

                    {/* 2. MAC PIPELINE: CASH & CAPITAL ECONOMICS */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-emerald-600 w-2 h-6 mr-3 rounded-sm"></span>
                            MAC Pipeline: Cash & Capital Economics (2025)
                        </h2>
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                            <div className="h-80 w-full">
                                <ResponsiveContainer width="100%" height="100%">
                                    <ComposedChart
                                        data={cashEconomicsData}
                                        margin={{ top: 20, right: 30, left: 20, bottom: 5 }}
                                    >
                                        <CartesianGrid strokeDasharray="3 3" vertical={false} />
                                        <XAxis dataKey="month" tick={{fill: '#64748b'}} />
                                        {/* Added Y-Axis Label */}
                                        <YAxis tick={{fill: '#64748b'}} tickFormatter={(val) => `$${val/1000}k`} label={{ value: 'Cash Flow ($)', angle: -90, position: 'insideLeft', fill: '#94a3b8' }} />
                                        <Tooltip formatter={(value) => formatCurrency(value)} contentStyle={{borderRadius: '8px', border: 'none', boxShadow: '0 4px 6px -1px rgb(0 0 0 / 0.1)'}} />
                                        <Legend />
                                        <Bar dataKey="AppFees" stackId="a" fill="#a7f3d0" name="App Fees" />
                                        <Bar dataKey="Deposits" stackId="a" fill="#34d399" name="Deposits" />
                                        <Bar dataKey="Capital" stackId="a" fill="#059669" name="Capital Funds" radius={[4, 4, 0, 0]} />
                                        <Line type="monotone" dataKey="Total" stroke="#064e3b" strokeWidth={3} dot={{r: 4}} name="Total Entry Cash" />
                                    </ComposedChart>
                                </ResponsiveContainer>
                            </div>
                        </div>
                    </div>

                    {/* 1. MAC PIPELINE: STAGE BREAKDOWN */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-slate-800 w-2 h-6 mr-3 rounded-sm"></span>
                            MAC Pipeline: Stage Breakdown Lookback YTD 2025
                        </h2>
                        <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                            <p className="text-sm text-slate-500 mb-4 leading-relaxed">
                                Monthly snapshot of the candidate pipeline volume across all stages throughout 2025.
                            </p>
                            <div className="h-80 w-full">
                                <ResponsiveContainer width="100%" height="100%">
                                    <BarChart
                                        data={pipelineHistoryData}
                                        margin={{ top: 20, right: 30, left: 20, bottom: 5 }}
                                    >
                                        <CartesianGrid strokeDasharray="3 3" vertical={false} />
                                        <XAxis dataKey="month" tick={{fill: '#64748b'}} />
                                        {/* Added Y-Axis Label */}
                                        <YAxis tick={{fill: '#64748b'}} label={{ value: 'Volume (Candidates)', angle: -90, position: 'insideLeft', fill: '#94a3b8' }} />
                                        <Tooltip cursor={{fill: '#f1f5f9'}} contentStyle={{borderRadius: '8px', border: 'none', boxShadow: '0 4px 6px -1px rgb(0 0 0 / 0.1)'}} />
                                        {/* Use custom legend to match Top-Down stack order visual preference */}
                                        <Legend payload={pipelineLegend} />
                                        {/* Render Invited first (Bottom) -> Applicants last (Top) */}
                                        <Bar dataKey="Invited" stackId="a" fill="#1d4ed8" name="Invited" />
                                        <Bar dataKey="Committee" stackId="a" fill="#2563eb" name="Cmte. Review" />
                                        <Bar dataKey="Processing" stackId="a" fill="#3b82f6" name="In Processing" />
                                        <Bar dataKey="Waitlist" stackId="a" fill="#60a5fa" name="Waitlist" />
                                        <Bar dataKey="Applicants" stackId="a" fill="#94a3b8" name="Applicants" radius={[4, 4, 0, 0]} />
                                    </BarChart>
                                </ResponsiveContainer>
                            </div>
                        </div>
                    </div>

                    {/* 3. PIPELINE FLOW INFOGRAPHIC (Replaces the Chart) */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-purple-600 w-2 h-6 mr-3 rounded-sm"></span>
                            Pipeline Flow Dynamics & Lifecycle
                        </h2>
                        {/* Insert Custom Infographic Component */}
                        <PipelineCycleInfographic />
                        {/* Insert Historical Lookback Component */}
                        <LifecycleLookback />
                    </div>

                    {/* --- COMMITTEE BUSINESS SECTION --- */}
                    <div className="mb-12">
                        <h2 className="text-xl font-bold text-slate-800 mb-6 flex items-center">
                            <span className="bg-indigo-600 w-2 h-6 mr-3 rounded-sm"></span>
                            Committee Updates & Business
                        </h2>
                        
                        {/* EXISTING 3 COLUMNS */}
                        <div className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
                            <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                                <div className="flex items-center mb-4">
                                    <Activity className="w-5 h-5 text-indigo-600 mr-2" />
                                    <h3 className="font-bold text-slate-900">Strategic Initiatives</h3>
                                </div>
                                <ul className="space-y-4">
                                    <li className="text-sm text-slate-600">
                                        <span className="font-semibold text-slate-900 block mb-1">Attrition Anticipation (Retention)</span>
                                        <ul className="list-disc pl-4 space-y-1 mt-1">
                                            <li><strong>Metabolic Rate:</strong> Historical data projects a natural attrition of ~53 resignations/month.</li>
                                            <li><strong>Driving Forces:</strong> Member disengagement ("Nonuse") and relocation ("Moved Away") were the primary drivers behind the majority of resignations.</li>
                                        </ul>
                                    </li>
                                    <li className="text-sm text-slate-600">
                                        <span className="font-semibold text-slate-900 block mb-1">Proposer Recognition</span>
                                        Program approved by Board of Trustees; implementation phase is currently in progress. Communications and Membership are developing the promotions and launch materials.
                                        <span className="block mt-2 font-bold text-emerald-600 text-xs uppercase tracking-wide">Goal: Increase pipeline accounts by 40%</span>
                                    </li>
                                </ul>
                            </div>

                            <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                                <div className="flex items-center mb-4">
                                    <BookOpen className="w-5 h-5 text-blue-600 mr-2" />
                                    <h3 className="font-bold text-slate-900">New Business (5 min)</h3>
                                </div>
                                <ul className="space-y-4">
                                    <li className="text-sm text-slate-600">
                                        <span className="font-semibold text-slate-900 block mb-1">Redline Membership P&P</span>
                                        Request to accept housekeeping updates aligning P&P with current Club Rules and forms. Edits focus on "At Your Service" nomenclature updates and consistency regarding Nonresident property ownership definitions.
                                    </li>
                                    <li className="text-sm text-slate-600">
                                        <span className="font-semibold text-slate-900 block mb-1">Policy Review: Honorary Retention</span>
                                        Review and introduce a line item in medical inactive policy for terminal members.
                                    </li>
                                </ul>
                            </div>

                            <div className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                                <div className="flex items-center mb-4">
                                    <Clock className="w-5 h-5 text-slate-500 mr-2" />
                                    <h3 className="font-bold text-slate-900">Old Business (5 min)</h3>
                                </div>
                                <ul className="space-y-4">
                                    <li className="text-sm text-slate-600">
                                        <span className="font-semibold text-slate-900 block mb-1">Initiation Fee Audit Update</span>
                                        Full account audit is complete. Staff has moved to the individual outreach phase through December, with a target of final case resolutions and action plans in place by January.
                                    </li>
                                </ul>
                            </div>
                        </div>

                         {/* ... Strategic Roadmap & Retention Risk Radar ... */}
                        <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
                            {/* ... (Roadmap & Radar content remains the same) ... */}
                            <div className="lg:col-span-2 bg-white rounded-xl border border-slate-200 shadow-sm p-6">
                                <div className="flex items-center mb-6 pb-4 border-b border-slate-100">
                                    <MapPin className="w-6 h-6 text-emerald-600 mr-3" />
                                    <div>
                                        <h3 className="text-lg font-bold text-slate-900">Strategic Roadmap: 2025 Outcomes & 2026 Focus</h3>
                                        <p className="text-sm text-slate-500">Initiative tracking and forward-looking strategy</p>
                                    </div>
                                </div>

                                <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
                                    {/* 2025 Completed */}
                                    <div>
                                        <h4 className="text-xs font-bold text-emerald-600 uppercase tracking-widest mb-4">2025 Completed</h4>
                                        <ul className="space-y-4">
                                            <li className="flex items-start">
                                                <CheckCircle className="w-5 h-5 text-emerald-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Intermediate "Earn-Down"</span>
                                                    <span className="text-xs text-slate-500">Pipeline action driver & Legacy retention.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <CheckCircle className="w-5 h-5 text-emerald-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Unified Monthly Billing</span>
                                                    <span className="text-xs text-slate-500">Standardized revenue flow.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <CheckCircle className="w-5 h-5 text-emerald-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Initiation Fee ($7k)</span>
                                                    <span className="text-xs text-slate-500">Increased capital contribution.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <CheckCircle className="w-5 h-5 text-emerald-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">"Family of 2" Launch</span>
                                                    <span className="text-xs text-slate-500">Retention firewall for empty nesters.</span>
                                                </div>
                                            </li>
                                             <li className="flex items-start">
                                                <CheckCircle className="w-5 h-5 text-emerald-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Return of Junior Quizzes</span>
                                                    <span className="text-xs text-slate-500">Club returned to requesting juniors to complete quizzes at ages 7, 11, and 14.</span>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>

                                    {/* 2026 Strategic Focus */}
                                    <div>
                                        <h4 className="text-xs font-bold text-blue-600 uppercase tracking-widest mb-4">2026 Strategic Focus</h4>
                                        <ul className="space-y-4">
                                            <li className="flex items-start">
                                                <ArrowRight className="w-5 h-5 text-blue-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Ambassador Activation (Proposer Recognition)</span>
                                                    <span className="text-xs text-slate-500">Move beyond passive referrals. Actively celebrate "Ambassador" members.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <ArrowRight className="w-5 h-5 text-blue-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Attrition Anticipation (Retention)</span>
                                                    <span className="text-xs text-slate-500">Shift from reactive to proactive identification of declining usage patterns.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <Star className="w-5 h-5 text-amber-500 mr-2 flex-shrink-0 mt-0.5 fill-current" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">135th Anniversary Campaign</span>
                                                    <span className="text-xs text-slate-500">Capitalize on the milestone to push hard core themes.</span>
                                                </div>
                                            </li>
                                            <li className="flex items-start">
                                                <ArrowRight className="w-5 h-5 text-blue-500 mr-2 flex-shrink-0 mt-0.5" />
                                                <div>
                                                    <span className="font-bold text-slate-800 block text-sm">Lifelong Athlete Program</span>
                                                    <span className="text-xs text-slate-500">Leverage program for re-onboarding ramps.</span>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                </div>

                                {/* Operational Excellence */}
                                <div className="mt-8 pt-6 border-t border-slate-100">
                                    <h4 className="text-xs font-bold text-slate-400 uppercase tracking-widest mb-4">Operational Excellence</h4>
                                    <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                                        <div className="flex items-start">
                                            <Settings className="w-5 h-5 text-slate-400 mr-2 flex-shrink-0 mt-0.5" />
                                            <div>
                                                <span className="font-bold text-slate-800 block text-sm">Digitization & Automation</span>
                                                <span className="text-xs text-slate-500">DocuSign for Esignature of everyday forms and Communications Campaigns.</span>
                                            </div>
                                        </div>
                                        <div className="flex items-start">
                                            <Settings className="w-5 h-5 text-slate-400 mr-2 flex-shrink-0 mt-0.5" />
                                            <div>
                                                <span className="font-bold text-slate-800 block text-sm">Pipeline Champions</span>
                                                <span className="text-xs text-slate-500">Operational Membership Specialists with quarterly "focus" on tailored pathways.</span>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            {/* RETENTION RISK RADAR (Right col) */}
                            <div className="bg-slate-50 rounded-xl border border-slate-200 shadow-sm p-6 flex flex-col">
                                <div className="flex items-center mb-6 pb-2 border-b border-slate-200">
                                    <Target className="w-6 h-6 text-red-500 mr-3" />
                                    <h3 className="text-lg font-bold text-slate-900">Retention Risk Radar (DRAFT)</h3>
                                </div>
                                <p className="text-sm text-slate-500 mb-4 leading-relaxed">Example mockup of engagement connection opportunities. To be further developed by Drop Points & Retention Subcommittee.</p>

                                <div className="space-y-6 flex-grow">
                                    {/* Item 1 */}
                                    <div className="bg-white p-4 rounded-lg border-l-4 border-red-500 shadow-sm">
                                        <div className="flex justify-between items-start mb-1">
                                            <span className="text-xs font-bold text-red-600 uppercase">High Risk</span>
                                            <span className="text-xl font-black text-slate-800">145</span>
                                        </div>
                                        <h4 className="font-bold text-slate-900 text-sm">The "Senior Cliff"</h4>
                                        <p className="text-xs text-slate-500 mt-1">Sudden drop from high usage to zero. Indicates health event.</p>
                                        <div className="mt-2 text-[10px] text-slate-400 font-semibold">At-Risk Seniors (>75)</div>
                                    </div>

                                    {/* Item 2 */}
                                    <div className="bg-white p-4 rounded-lg border-l-4 border-amber-500 shadow-sm">
                                        <div className="flex justify-between items-start mb-1">
                                            <span className="text-xs font-bold text-amber-600 uppercase">Med Risk</span>
                                            <span className="text-xl font-black text-slate-800">82</span>
                                        </div>
                                        <h4 className="font-bold text-slate-900 text-sm">"Silent Lapsers" (Age 26)</h4>
                                        <p className="text-xs text-slate-500 mt-1">Disengagement 3-6 months before dues jump.</p>
                                        <div className="mt-2 text-[10px] text-slate-400 font-semibold">Intermediates approaching 26</div>
                                    </div>

                                    {/* Item 3 */}
                                    <div className="bg-white p-4 rounded-lg border-l-4 border-slate-400 shadow-sm">
                                        <div className="flex justify-between items-start mb-1">
                                            <span className="text-xs font-bold text-slate-500 uppercase">Low Value</span>
                                            <span className="text-xl font-black text-slate-800">215</span>
                                        </div>
                                        <h4 className="font-bold text-slate-900 text-sm">Ghost Members</h4>
                                        <p className="text-xs text-slate-500 mt-1">New members (&lt;1 yr) with zero usage in 30 days.</p>
                                        <div className="mt-2 text-[10px] text-slate-400 font-semibold">Failure to Launch</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            );
        };

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<MembershipDashboard />);
    </script>
</body>
</html>
