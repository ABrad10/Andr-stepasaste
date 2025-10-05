<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Monitor Fenológico - Cerro de Pasco</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #0a0e1a;
            color: #fff;
            overflow: hidden;
        }

        .container {
            display: flex;
            height: 100vh;
            position: relative;
        }

        /* Sidebar */
        .sidebar {
            width: 80px;
            background: rgba(20, 25, 40, 0.95);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px 0;
            gap: 15px;
            border-right: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 10;
        }

        .logo-btn {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 18px;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .logo-btn:hover {
            transform: scale(1.1);
        }

        .sidebar-btn {
            width: 50px;
            height: 50px;
            background: rgba(255, 255, 255, 0.1);
            border: none;
            border-radius: 10px;
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 5px;
            transition: all 0.3s;
            color: #fff;
        }

        .sidebar-btn:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateX(5px);
        }

        .sidebar-btn svg {
            width: 24px;
            height: 24px;
        }

        .btn-label {
            font-size: 8px;
            text-transform: uppercase;
        }

        .report-btn {
            background: #dc2626;
            margin-top: auto;
        }

        /* Main Content */
        .main-content {
            flex: 1;
            position: relative;
            overflow: hidden;
        }

        /* Map Container */
        .map-container {
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #1a2332 0%, #0f1419 100%);
            position: relative;
            overflow: hidden;
        }

        .map-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.7;
            transition: transform 0.3s ease;
        }

        /* Markers */
        .marker {
            position: absolute;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: transform 0.3s;
            animation: pulse 2s infinite;
            z-index: 2;
            font-size: 24px;
            border: 3px solid white;
            box-shadow: 0 4px 8px rgba(0,0,0,0.3);
        }

        .marker:hover {
            transform: scale(1.3);
            z-index: 5;
        }

        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 0 0 rgba(255, 255, 255, 0.7); }
            50% { box-shadow: 0 0 0 10px rgba(255, 255, 255, 0); }
        }

        .marker.restringida { background: #fbbf24; }
        .marker.area-verde { background: #10b981; }
        .marker.saludable { background: #059669; }
        .marker.contaminada { background: #dc2626; }
        .marker.mineria { background: #8b5cf6; }
        .marker.incendio { background: #ef4444; }

        /* Info Panel - Más compacto */
.info-panel {
    position: absolute;
    bottom: 15px;
    left: 100px;
    background: rgba(20, 25, 40, 0.95);
    padding: 15px; /* Más reducido */
    border-radius: 12px;
    min-width: 280px; /* Más pequeño */
    max-width: 320px; /* Más pequeño */
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    z-index: 10;
}

.character {
    width: 90px; /* Más pequeño */
    height: 90px;
    position: absolute;
    bottom: 10px;
    left: -100px;
}

        .info-text h3 {
            color: #10b981;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .info-text p {
            line-height: 1.6;
            color: #e5e7eb;
            margin-bottom: 15px;
        }

        .change-lang-btn {
            background: #10b981;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s;
        }

        .change-lang-btn:hover {
            background: #059669;
        }

        /* Reports Sidebar */
        .reports-sidebar {
            position: absolute;
            right: 0;
            top: 0;
            width: 350px;
            height: 100%;
            background: rgba(20, 25, 40, 0.95);
            padding: 20px;
            overflow-y: auto;
            border-left: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 10;
        }

        .reports-header {
            margin-bottom: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .reports-header h2 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .nasa-badge {
            background: linear-gradient(135deg, #1a5fb4, #0d2d5c);
            padding: 4px 8px;
            border-radius: 4px;
            font-size: 10px;
            font-weight: bold;
        }

        .live-indicator {
            display: flex;
            align-items: center;
            gap: 5px;
            color: #ef4444;
            font-size: 12px;
        }

        .live-dot {
            width: 8px;
            height: 8px;
            background: #ef4444;
            border-radius: 50%;
            animation: blink 1s infinite;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.3; }
        }

        .report-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.2s;
        }

        .report-card:hover {
            transform: translateY(-2px);
            background: rgba(255, 255, 255, 0.08);
        }

        .report-image {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 10px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .report-title {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 8px;
            color: #fff;
        }

        .report-location {
            font-size: 12px;
            color: #9ca3af;
            margin-bottom: 8px;
        }

        .report-nasa-info {
            font-size: 11px;
            color: #60a5fa;
            margin-bottom: 8px;
            line-height: 1.4;
        }

        .report-metrics {
            display: flex;
            gap: 10px;
            margin-bottom: 8px;
        }

        .metric {
            background: rgba(255, 255, 255, 0.1);
            padding: 4px 8px;
            border-radius: 4px;
            font-size: 10px;
        }

        .metric.high { background: rgba(239, 68, 68, 0.2); color: #fca5a5; }
        .metric.medium { background: rgba(245, 158, 11, 0.2); color: #fcd34d; }
        .metric.low { background: rgba(34, 197, 94, 0.2); color: #86efac; }

        .report-source {
            font-size: 10px;
            color: #6b7280;
            text-align: right;
        }

        /* Legend */
        .legend {
            position: absolute;
            top: 20px;
            left: 100px;
            background: rgba(20, 25, 40, 0.95);
            padding: 20px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 10;
        }

        .legend h3 {
            font-size: 14px;
            margin-bottom: 15px;
        }

        .legend-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 10px;
            font-size: 13px;
        }

        .legend-color {
            width: 20px;
            height: 20px;
            border-radius: 50%;
        }

        /* Modal for Logo Change */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 100;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: #1a2332;
            padding: 30px;
            border-radius: 15px;
            max-width: 500px;
            width: 90%;
        }

        .modal-content h2 {
            margin-bottom: 20px;
        }

        .modal-content input {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            border-radius: 8px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 14px;
        }

        .modal-buttons {
            display: flex;
            gap: 10px;
            justify-content: flex-end;
        }

        .modal-btn {
            padding: 10px 20px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s;
        }

        .modal-btn.cancel {
            background: #6b7280;
            color: white;
        }

        .modal-btn.save {
            background: #10b981;
            color: white;
        }

        .modal-btn:hover {
            opacity: 0.8;
        }

        /* Tooltip */
        .tooltip {
            position: absolute;
            background: rgba(0, 0, 0, 0.9);
            padding: 10px 15px;
            border-radius: 8px;
            font-size: 12px;
            pointer-events: none;
            display: none;
            z-index: 50;
            white-space: nowrap;
        }

        .tooltip.active {
            display: block;
        }

        /* Marker Info Panel */
        .marker-info-panel {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(20, 25, 40, 0.95);
            padding: 25px;
            border-radius: 15px;
            min-width: 400px;
            max-width: 500px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 20;
            display: none;
        }

        .marker-info-panel.active {
            display: block;
        }

        .marker-info-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .marker-info-title {
            font-size: 18px;
            font-weight: 600;
        }

        .close-btn {
            background: none;
            border: none;
            color: white;
            font-size: 20px;
            cursor: pointer;
        }

        .marker-info-content {
            margin-bottom: 15px;
        }

        .info-row {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .info-label {
            color: #9ca3af;
        }

        .info-value {
            font-weight: 600;
        }

        .sembrar-btn {
            background: #10b981;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s;
            width: 100%;
            margin-top: 10px;
        }

        .sembrar-btn:hover {
            background: #059669;
        }

        .sembrar-btn.disabled {
            background: #6b7280;
            cursor: not-allowed;
        }

        /* Map Controls */
        .map-controls {
            position: absolute;
            top: 20px;
            right: 370px;
            display: flex;
            gap: 10px;
            z-index: 10;
        }

        .control-btn {
            background: rgba(20, 25, 40, 0.95);
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.3s;
        }

        .control-btn:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .file-input {
            display: none;
        }

        .file-label {
            background: rgba(20, 25, 40, 0.95);
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: white;
            padding: 10px 15px;
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 14px;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .file-label:hover {
            background: rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Sidebar -->
        <div class="sidebar">
            <div class="logo-btn" onclick="openLogoModal()">
                <span id="logoText">FP</span>
            </div>

            <button class="sidebar-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"/>
                </svg>
                <span class="btn-label">Capas</span>
            </button>

            <button class="sidebar-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <path d="M14 2H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h12c1.1 0 2-.9 2-2V8l-6-6z"/>
                </svg>
                <span class="btn-label">Gaming</span>
            </button>

            <button class="sidebar-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <circle cx="12" cy="12" r="10"/>
                    <path d="M12 6v6l4 2" stroke="white" stroke-width="2" fill="none"/>
                </svg>
                <span class="btn-label">Tiempo</span>
            </button>

            <button class="sidebar-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5"/>
                </svg>
                <span class="btn-label">Report</span>
            </button>

            <button class="sidebar-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <path d="M20 2H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h14l4 4V4c0-1.1-.9-2-2-2z"/>
                </svg>
                <span class="btn-label">Chat</span>
            </button>

            <button class="sidebar-btn report-btn">
                <svg viewBox="0 0 24 24" fill="currentColor">
                    <path d="M1 21h22L12 2 1 21zm12-3h-2v-2h2v2zm0-4h-2v-4h2v4z"/>
                </svg>
                <span class="btn-label">Alerta</span>
            </button>
        </div>

        <!-- Main Content -->
        <div class="main-content">
            <div class="map-container" id="mapContainer">
                <!-- Map Controls -->
                <div class="map-controls">
                    <button class="control-btn" onclick="zoomIn()">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/>
                        </svg>
                    </button>
                    <button class="control-btn" onclick="zoomOut()">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M19 13H5v-2h14v2z"/>
                        </svg>
                    </button>
                    <button class="control-btn" onclick="resetZoom()">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M12 5V1L7 6l5 5V7c3.31 0 6 2.69 6 6s-2.69 6-6 6-6-2.69-6-6H4c0 4.42 3.58 8 8 8s8-3.58 8-8-3.58-8-8-8z"/>
                        </svg>
                    </button>
                    <label for="mapUpload" class="file-label">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/>
                        </svg>
                        Cargar Mapa
                    </label>
                    <input type="file" id="mapUpload" class="file-input" accept="image/*" onchange="loadMapImage(event)">
                </div>

                <!-- Map Image -->
                <img id="mapImage" class="map-image" src="" alt="Mapa de Cerro de Pasco">
                
                <!-- Default map if no image is loaded -->
                <svg id="defaultMap" class="map-image" viewBox="0 0 1200 800" preserveAspectRatio="xMidYMid slice">
                    <defs>
                        <linearGradient id="terrainGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#2d5016;stop-opacity:1" />
                            <stop offset="50%" style="stop-color:#4a7023;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#1a3a0f;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <!-- Terrain simulation -->
                    <rect width="1200" height="800" fill="url(#terrainGrad)"/>
                    <circle cx="300" cy="200" r="80" fill="#8b7355" opacity="0.6"/>
                    <circle cx="500" cy="400" r="120" fill="#6b5d4f" opacity="0.5"/>
                    <circle cx="800" cy="300" r="100" fill="#7a6a5a" opacity="0.6"/>
                    <path d="M 0 600 Q 300 550 600 580 T 1200 600 L 1200 800 L 0 800 Z" fill="#1e4d2b" opacity="0.7"/>
                    <text x="600" y="400" text-anchor="middle" fill="white" opacity="0.3" font-size="24">CERRO DE PASCO</text>
                </svg>

                <!-- Markers con Emojis Divertidos -->
                <!-- Zona protegida que SÍ permite siembra con permisos -->
                <div class="marker restringida" style="top: 25%; left: 30%;" 
                     data-info='{"title":"Zona Protegida - Reserva Paisajística","tipo":"Área protegida","superficie":"150 ha","tipoTierra":"Tierra fértil","magnitud":"N/A","mineriaIlegal":false,"incendio":false,"aptaSembrar":true,"permisoRequerido":true}'
                     onclick="showMarkerInfo(this)">
                    🏞️
                </div>

                <!-- Zona protegida que NO permite siembra -->
                <div class="marker restringida" style="top: 15%; left: 40%;" 
                     data-info='{"title":"Parque Nacional - Protección Estricta","tipo":"Parque nacional","superficie":"850 ha","tipoTierra":"Bosque primario","magnitud":"N/A","mineriaIlegal":false,"incendio":false,"aptaSembrar":false,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    🚫
                </div>

                <div class="marker area-verde" style="top: 35%; left: 55%;" 
                     data-info='{"title":"Área Verde Protegida","tipo":"Área verde","superficie":"320 ha","tipoTierra":"Bosque nativo","magnitud":"N/A","mineriaIlegal":false,"incendio":false,"aptaSembrar":true,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    🌳
                </div>

                <div class="marker saludable" style="top: 60%; left: 45%;" 
                     data-info='{"title":"Zona Agrícola Saludable","tipo":"Zona saludable","superficie":"85 ha","tipoTierra":"Tierra fértil","magnitud":"N/A","mineriaIlegal":false,"incendio":false,"aptaSembrar":true,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    🌱
                </div>

                <div class="marker contaminada" style="top: 45%; left: 70%;" 
                     data-info='{"title":"Zona Contaminada","tipo":"Zona contaminada","superficie":"210 ha","tipoTierra":"Suelo degradado","magnitud":"Alta","mineriaIlegal":false,"incendio":false,"aptaSembrar":false,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    ☠️
                </div>

                <div class="marker mineria" style="top: 50%; left: 25%;" 
                     data-info='{"title":"Zona con Minería Ilegal","tipo":"Minería ilegal","superficie":"45 ha","tipoTierra":"Suelo erosionado","magnitud":"Media","mineriaIlegal":true,"incendio":false,"aptaSembrar":false,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    ⛏️😢
                </div>

                <div class="marker incendio" style="top: 28%; left: 65%;" 
                     data-info='{"title":"Incendio Forestal Activo","tipo":"Incendio forestal","superficie":"120 ha","tipoTierra":"Bosque seco","magnitud":"Alta","mineriaIlegal":false,"incendio":true,"aptaSembrar":false,"permisoRequerido":false}'
                     onclick="showMarkerInfo(this)">
                    🔥😢
                </div>

                <!-- Legend -->
                <div class="legend">
                    <h3>Leyenda</h3>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #fbbf24;"></div>
                        <span>Zona Restringida</span>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #10b981;"></div>
                        <span>Área Verde</span>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #059669;"></div>
                        <span>Zona Saludable</span>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #dc2626;"></div>
                        <span>Zona Contaminada</span>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #8b5cf6;"></div>
                        <span>Minería Ilegal</span>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #ef4444;"></div>
                        <span>Incendio Forestal</span>
                    </div>
                </div>

                <!-- Info Panel -->
                <div class="info-panel">
                    <div class="character">
                        <svg viewBox="0 0 200 200" style="width: 100%; height: 100%;">
                            <ellipse cx="100" cy="160" rx="50" ry="20" fill="#2d5016" opacity="0.3"/>
                            <circle cx="100" cy="80" r="50" fill="#8b6f47"/>
                            <circle cx="85" cy="75" r="5" fill="#000"/>
                            <circle cx="115" cy="75" r="5" fill="#000"/>
                            <path d="M 85 95 Q 100 105 115 95" stroke="#000" stroke-width="2" fill="none"/>
                            <ellipse cx="100" cy="140" rx="40" ry="50" fill="#10b981"/>
                            <rect x="70" y="120" width="20" height="50" fill="#8b6f47"/>
                            <rect x="110" y="120" width="20" height="50" fill="#8b6f47"/>
                            <circle cx="65" cy="60" r="15" fill="#6b8e23"/>
                            <circle cx="135" cy="60" r="15" fill="#6b8e23"/>
                        </svg>
                    </div>
                    <div class="info-text">
                        <h3>¡Hola! Soy el Monitor Fenológico.</h3>
                        <p>Bienvenido a la plataforma de monitoreo fenológico de Cerro de Pasco, Perú. Aquí puedes visualizar problemas ambientales en tiempo real y recibir alertas sobre zonas restringidas, áreas verdes, zonas contaminadas y minería ilegal.</p>
                        <button class="change-lang-btn" onclick="changeLanguage()">Cambiar Idioma</button>
                    </div>
                </div>

                <!-- Marker Info Panel -->
                <div class="marker-info-panel" id="markerInfoPanel">
                    <div class="marker-info-header">
                        <div class="marker-info-title" id="markerTitle">Título del Marcador</div>
                        <button class="close-btn" onclick="closeMarkerInfo()">×</button>
                    </div>
                    <div class="marker-info-content">
                        <div class="info-row">
                            <span class="info-label">Tipo:</span>
                            <span class="info-value" id="infoTipo">-</span>
                        </div>
                        <div class="info-row">
                            <span class="info-label">Superficie:</span>
                            <span class="info-value" id="infoSuperficie">-</span>
                        </div>
                        <div class="info-row">
                            <span class="info-label">Tipo de Tierra:</span>
                            <span class="info-value" id="infoTipoTierra">-</span>
                        </div>
                        <div class="info-row">
                            <span class="info-label">Magnitud:</span>
                            <span class="info-value" id="infoMagnitud">-</span>
                        </div>
                        <div class="info-row">
                            <span class="info-label">Minería Ilegal:</span>
                            <span class="info-value" id="infoMineria">-</span>
                        </div>
                        <div class="info-row">
                            <span class="info-label">Incendio Forestal:</span>
                            <span class="info-value" id="infoIncendio">-</span>
                        </div>
                    </div>
                    <button class="sembrar-btn" id="sembrarBtn">Evaluar para Siembra</button>
                </div>
            </div>

            <!-- Reports Sidebar con Imágenes y Datos NASA -->
            <div class="reports-sidebar">
                <div class="reports-header">
                    <div>
                        <h2>Reportes de Hoy</h2>
                        <div class="live-indicator">
                            <div class="live-dot"></div>
                            <span>En Vivo - Datos NASA</span>
                        </div>
                    </div>
                    <div class="nasa-badge">NASA</div>
                </div>

                <!-- Reporte 1: Incendio Forestal -->
                <div class="report-card">
                    <img src="descarga.jpeg" alt="Incendio forestal" class="report-image">
                    <div class="report-title">🔥 Incendio Forestal Activo - Cerro de Pasco</div>
                    <div class="report-location">📍 Distrito de Yanacancha, Región Pasco</div>
                    <div class="report-nasa-info">
                        🛰️ <strong>NASA FIRMS:</strong> Detección de puntos calientes activos. Temperatura superficial: 85°C. Área afectada: 120 hectáreas.
                    </div>
                    <div class="report-metrics">
                        <div class="metric high">Riesgo Alto</div>
                        <div class="metric">CO2: 450 ppm</div>
                        <div class="metric">Vientos: 25 km/h</div>
                    </div>
                    <div class="report-source">Fuente: NASA FIRMS - MODIS/Terra - Actualizado: Hoy 14:30</div>
                </div>

                <!-- Reporte 2: Minería Ilegal -->
                <div class="report-card">
                    <img src="https://images.unsplash.com/photo-1585970480901-90d6bb2a48b5?w=400&h=200&fit=crop" alt="Minería ilegal" class="report-image">
                    <div class="report-title">⛏️ Actividad Minera Ilegal Detectada</div>
                    <div class="report-location">📍 Zona de Simón Bolívar, Cerro de Pasco</div>
                    <div class="report-nasa-info">
                        🛰️ <strong>NASA Landsat 9:</strong> Cambios en reflectividad del suelo. Detección de excavaciones no autorizadas. Área afectada: 45 hectáreas.
                    </div>
                    <div class="report-metrics">
                        <div class="metric medium">Impacto Medio</div>
                        <div class="metric">Mercurio: 0.8 ppm</div>
                        <div class="metric">Sedimentos: Alto</div>
                    </div>
                    <div class="report-source">Fuente: NASA Landsat 9 - Actualizado: Hoy 11:15</div>
                </div>

                <!-- Reporte 3: Sequía Severa -->
                <div class="report-card">
                    <img src="https://images.unsplash.com/photo-1509316785289-025f5b846b35?w=400&h=200&fit=crop" alt="Sequía severa" class="report-image">
                    <div class="report-title">🏜️ Sequía Severa en Zona Altiplánica</div>
                    <div class="report-location">📍 Meseta del Bombón, Junín</div>
                    <div class="report-nasa-info">
                        🛰️ <strong>NASA GRACE-FO:</strong> Disminución del almacenamiento de agua subterránea. Índice de vegetación (NDVI) en niveles críticos.
                    </div>
                    <div class="report-metrics">
                        <div class="metric high">Sequía Extrema</div>
                        <div class="metric">Humedad: 12%</div>
                        <div class="metric">NDVI: 0.15</div>
                    </div>
                    <div class="report-source">Fuente: NASA GRACE-FO - Actualizado: Hoy 09:45</div>
                </div>

                <!-- Reporte 4: Calidad del Aire -->
                <div class="report-card">
                    <img src="https://images.unsplash.com/photo-1563453392212-326f5e854473?w=400&h=200&fit=crop" alt="Contaminación aire" class="report-image">
                    <div class="report-title">🌫️ Alta Contaminación Atmosférica</div>
                    <div class="report-location">📍 Ciudad de Cerro de Pasco</div>
                    <div class="report-nasa-info">
                        🛰️ <strong>NASA AURA:</strong> Niveles elevados de SO2 y partículas PM2.5. Concentración: 45 μg/m³ (OMS: 25 μg/m³).
                    </div>
                    <div class="report-metrics">
                        <div class="metric high">Calidad Mala</div>
                        <div class="metric">PM2.5: 45 μg/m³</div>
                        <div class="metric">SO2: 12 ppb</div>
                    </div>
                    <div class="report-source">Fuente: NASA AURA/OMI - Actualizado: Hoy 16:20</div>
                </div>

                <!-- Reporte 5: Deforestación -->
                <div class="report-card">
                    <img src="https://images.unsplash.com/photo-1614583225154-5fcdda07019e?w=400&h=200&fit=crop" alt="Deforestación" class="report-image">
                    <div class="report-title">🌳 Pérdida de Cobertura Forestal</div>
                    <div class="report-location">📍 Bosque de Huayllay</div>
                    <div class="report-nasa-info">
                        🛰️ <strong>NASA GEDI:</strong> Pérdida de 320 hectáreas de bosque en último trimestre. Altura de dosel reducida en 35%.
                    </div>
                    <div class="report-metrics">
                        <div class="metric high">Pérdida Alta</div>
                        <div class="metric">-320 ha</div>
                        <div class="metric">Carbono: -45K t</div>
                    </div>
                    <div class="report-source">Fuente: NASA GEDI - Actualizado: Ayer 18:30</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Tooltip -->
    <div class="tooltip" id="tooltip"></div>

    <!-- Logo Change Modal -->
    <div class="modal" id="logoModal">
        <div class="modal-content">
            <h2>Personalizar Logo</h2>
            <input type="text" id="logoInput" placeholder="Ingrese texto del logo (máx. 3 caracteres)" maxlength="3">
            <input type="color" id="colorInput" value="#667eea">
            <div class="modal-buttons">
                <button class="modal-btn cancel" onclick="closeLogoModal()">Cancelar</button>
                <button class="modal-btn save" onclick="saveLogo()">Guardar</button>
            </div>
        </div>
    </div>

    <script>
        // Logo customization
        function openLogoModal() {
            document.getElementById('logoModal').classList.add('active');
        }

        function closeLogoModal() {
            document.getElementById('logoModal').classList.remove('active');
        }

        function saveLogo() {
            const text = document.getElementById('logoInput').value.toUpperCase() || 'FP';
            const color = document.getElementById('colorInput').value;
            
            const logoBtn = document.querySelector('.logo-btn');
            logoBtn.style.background = `linear-gradient(135deg, ${color} 0%, ${adjustColor(color, -20)} 100%)`;
            document.getElementById('logoText').textContent = text;
            
            closeLogoModal();
        }

        function adjustColor(color, percent) {
            const num = parseInt(color.replace("#",""), 16);
            const amt = Math.round(2.55 * percent);
            const R = (num >> 16) + amt;
            const G = (num >> 8 & 0x00FF) + amt;
            const B = (num & 0x0000FF) + amt;
            return "#" + (0x1000000 + (R<255?R<1?0:R:255)*0x10000 +
                (G<255?G<1?0:G:255)*0x100 + (B<255?B<1?0:B:255))
                .toString(16).slice(1);
        }

        // Marker interactions
        function showMarkerInfo(marker) {
            const info = JSON.parse(marker.getAttribute('data-info'));
            const panel = document.getElementById('markerInfoPanel');
            
            document.getElementById('markerTitle').textContent = info.title;
            document.getElementById('infoTipo').textContent = info.tipo;
            document.getElementById('infoSuperficie').textContent = info.superficie;
            document.getElementById('infoTipoTierra').textContent = info.tipoTierra;
            document.getElementById('infoMagnitud').textContent = info.magnitud;
            document.getElementById('infoMineria').textContent = info.mineriaIlegal ? "Sí" : "No";
            document.getElementById('infoIncendio').textContent = info.incendio ? "Sí" : "No";
            
            const sembrarBtn = document.getElementById('sembrarBtn');
            if (info.aptaSembrar) {
                if (info.permisoRequerido) {
                    sembrarBtn.textContent = "Apta con Permiso Especial";
                    sembrarBtn.classList.remove('disabled');
                    sembrarBtn.onclick = function() { 
                        alert("Esta zona protegida permite agricultura sostenible pero requiere permisos especiales del gobierno."); 
                    };
                } else {
                    sembrarBtn.textContent = "Apta para Siembra";
                    sembrarBtn.classList.remove('disabled');
                    sembrarBtn.onclick = function() { 
                        alert("Esta zona es apta para actividades agrícolas."); 
                    };
                }
            } else {
                sembrarBtn.textContent = "No Apta para Siembra";
                sembrarBtn.classList.add('disabled');
                sembrarBtn.onclick = null;
            }
            
            panel.classList.add('active');
        }

        function closeMarkerInfo() {
            document.getElementById('markerInfoPanel').classList.remove('active');
        }

        // Tooltip
        const markers = document.querySelectorAll('.marker');
        const tooltip = document.getElementById('tooltip');

        markers.forEach(marker => {
            marker.addEventListener('mouseenter', (e) => {
                const info = JSON.parse(marker.getAttribute('data-info'));
                tooltip.textContent = info.title;
                tooltip.classList.add('active');
            });

            marker.addEventListener('mousemove', (e) => {
                tooltip.style.left = e.pageX + 15 + 'px';
                tooltip.style.top = e.pageY + 15 + 'px';
            });

            marker.addEventListener('mouseleave', () => {
                tooltip.classList.remove('active');
            });
        });

        // Language toggle
        let currentLang = 'es';
        function changeLanguage() {
            if (currentLang === 'es') {
                currentLang = 'en';
                document.querySelector('.info-text h3').textContent = 'Hello! I am the Phenological Monitor';
                document.querySelector('.info-text p').textContent = 'Welcome to the phenological monitoring platform for Cerro de Pasco, Peru. Here you can visualize environmental problems in real time and receive alerts about restricted areas, green areas, contaminated areas and illegal mining.';
                document.querySelector('.change-lang-btn').textContent = 'Change Language';
                document.querySelector('.reports-header h2').textContent = "Today's Reports";
                document.querySelector('.live-indicator span').textContent = "Live - NASA Data";
                document.querySelector('.legend h3').textContent = "Legend";
                document.querySelectorAll('.legend-item span')[0].textContent = "Restricted Area";
                document.querySelectorAll('.legend-item span')[1].textContent = "Green Area";
                document.querySelectorAll('.legend-item span')[2].textContent = "Healthy Area";
                document.querySelectorAll('.legend-item span')[3].textContent = "Contaminated Area";
                document.querySelectorAll('.legend-item span')[4].textContent = "Illegal Mining";
                document.querySelectorAll('.legend-item span')[5].textContent = "Forest Fire";
            } else {
                currentLang = 'es';
                document.querySelector('.info-text h3').textContent = '¡Hola! Soy el Monitor Fenológico';
                document.querySelector('.info-text p').textContent = 'Bienvenido a la plataforma de monitoreo fenológico de Cerro de Pasco, Perú. Aquí puedes visualizar problemas ambientales en tiempo real y recibir alertas sobre zonas restringidas, áreas verdes, zonas contaminadas y minería ilegal.';
                document.querySelector('.change-lang-btn').textContent = 'Cambiar Idioma';
                document.querySelector('.reports-header h2').textContent = "Reportes de Hoy";
                document.querySelector('.live-indicator span').textContent = "En Vivo - Datos NASA";
                document.querySelector('.legend h3').textContent = "Leyenda";
                document.querySelectorAll('.legend-item span')[0].textContent = "Zona Restringida";
                document.querySelectorAll('.legend-item span')[1].textContent = "Área Verde";
                document.querySelectorAll('.legend-item span')[2].textContent = "Zona Saludable";
                document.querySelectorAll('.legend-item span')[3].textContent = "Zona Contaminada";
                document.querySelectorAll('.legend-item span')[4].textContent = "Minería Ilegal";
                document.querySelectorAll('.legend-item span')[5].textContent = "Incendio Forestal";
            }
        }

        // Map zoom functionality
        let currentScale = 1;
        const mapImage = document.getElementById('mapImage');
        const defaultMap = document.getElementById('defaultMap');

        function zoomIn() {
            currentScale += 0.2;
            applyZoom();
        }

        function zoomOut() {
            if (currentScale > 0.4) {
                currentScale -= 0.2;
                applyZoom();
            }
        }

        function resetZoom() {
            currentScale = 1;
            applyZoom();
        }

        function applyZoom() {
            mapImage.style.transform = `scale(${currentScale})`;
            defaultMap.style.transform = `scale(${currentScale})`;
        }

        // Load custom map image
        function loadMapImage(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    mapImage.src = e.target.result;
                    mapImage.style.display = 'block';
                    defaultMap.style.display = 'none';
                };
                reader.readAsDataURL(file);
            }
        }

        // Initialize with default map
        window.onload = function() {
            defaultMap.style.display = 'block';
            mapImage.style.display = 'none';
        };
    </script>
</body>
</html>
