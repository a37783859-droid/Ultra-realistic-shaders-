-- Super Realistic Shaders Script
-- Настройки освещения и пост-обработки

local Lighting = game:GetService("Lighting")
local Terrain = game:GetService("Workspace").Terrain

-- 1. Базовые настройки движка на максимум
Lighting.GlobalShadows = true
Lighting.ShadowSoftness = 0 -- Делает тени четкими и реалистичными
Lighting.EnvironmentDiffuseScale = 1
Lighting.EnvironmentSpecularScale = 1
Lighting.Technology = Enum.Technology.Future -- Включает самый мощный движок освещения

-- 2. Эффект Солнечных лучей (SunRays)
local sunRays = Instance.new("SunRaysEffect", Lighting)
sunRays.Intensity = 0.25
sunRays.Spread = 0.8

-- 3. Цветокоррекция (ColorCorrection) - делает картинку "сочной"
local colorCorrection = Instance.new("ColorCorrectionEffect", Lighting)
colorCorrection.Brightness = 0.05
colorCorrection.Contrast = 0.2
colorCorrection.Saturation = 0.15
colorCorrection.TintColor = Color3.fromRGB(255, 245, 230) -- Теплый оттенок

-- 4. Bloom (Свечение ярких объектов)
local bloom = Instance.new("BloomEffect", Lighting)
bloom.Intensity = 0.6
bloom.Size = 24
bloom.Threshold = 0.9

-- 5. Атмосфера (Имитация Volumetric Lighting / Туман)
local atmosphere = Instance.new("Atmosphere", Lighting)
atmosphere.Density = 0.35 -- Плотность воздуха (создает видимые лучи)
atmosphere.Glare = 2.5    -- Блики на солнце
atmosphere.Haze = 1.5     -- Дымка вдали
atmosphere.Color = Color3.fromRGB(190, 190, 190)
atmosphere.Decay = Color3.fromRGB(100, 100, 120)

-- 6. Размытие в движении (Motion Blur)
local blur = Instance.new("BlurEffect", Lighting)
blur.Size = 2 -- Легкое размытие для мягкости картинки

print("Ultra Realistic Shaders Loaded Successfully!")
