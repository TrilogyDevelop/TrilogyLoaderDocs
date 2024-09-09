Функции для работы с рендером
Функция рендера, например renderAddLine !!!ОБЯЗАТЕЛЬНО!!! вызвается только 1 раз, после чего все время на экране будет отрисовываться линия. Любая функция рендера (кроме renderEnd) возвращает уникальный идентификатор (nId). Чтобы завершить отрисовку любого объекта, вызывайте renderEnd(nId) которая принимает уникальный идентификатор отрисованного объекта, в нашем случае renderAddLine;

local nId = renderAddLine(float x1, float y1, float x2, float y2, int color, float thickness);
local nId = renderAddRect(float p_minX, float p_minY, float p_maxX, float p_maxY, int col, float rounding, Flags flags, float thickness);
local nId = renderAddRectFilled(float p_minX, float p_minY, float p_maxX, float p_maxY, int col, float rounding, Flags flags);
local nId = renderAddRectFilledMultiColor(float p_minX, float p_minY, float p_maxX, float p_maxY, int col_upr_left, int col_upr_right, int col_bot_right, int col_bot_left);
local nId = renderAddQuad(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, float pX4, float pY4, int col, float thickness);
local nId = renderAddQuadFilled(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, float pX4, float pY4, int col);
local nId = renderAddTriangle(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, int col, float thickness);
local nId = renderAddTriangleFilled(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, int col);
local nId = renderAddCircle(float centerX, float centerY, float radius, int col, int num_segments, float thickness);
local nId = renderAddCircleFilled(float centerX, float centerY, float radius, int col, int num_segments);
local nId = renderAddNgon(float centerX, float centerY, float radius, int col, int num_segments, float thickness);
local nId = renderAddNgonFilled(float centerX, float centerY, float radius, int col, int num_segments);
local nId = renderAddEllipse(float centerX, float centerY, float radius, int col, float rot, int num_segments, float thickness);
local nId = renderAddEllipseFilled(float centerX, float centerY, float radius, int col, float rot, int num_segments);
local nId = renderAddBezierCubic(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, float pX4, float pY4, int col, float thickness, int num_segments);
local nId = renderAddBezierQuadratic(float pX1, float pY1, float pX2, float pY2, float pX3, float pY3, int col, float thickness, int num_segments);
local nId = renderAddText(float X, float Y, int col, float font_size, String text);
renderEnd(int nIn);
