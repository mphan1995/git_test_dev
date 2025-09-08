# Quy trình & SLA cho Issues

## Trạng thái chính
- `triage` → `in progress` → `in review` → `done`

## SLA (tham khảo)
- **Bug – severity:critical**: nhận trong 1h, workaround < 4h, fix < 24h.
- **Bug – high**: nhận trong 4h, fix < 3 ngày.
- **Feature/Task**: xác nhận trong 1 ngày, lịch triển khai theo kế hoạch.

## Phân loại
- Dùng nhãn: `type/bug`, `type/feature`, `type/task`, `type/incident`
- Mức độ: `sev/critical`, `sev/high`, `sev/medium`, `sev/low`
- Khu vực: `area/frontend`, `area/backend`, `area/infra`, `area/docs`

## Chu kỳ tự động
- Tự gán `needs/triage` khi tạo.
- Thiếu thông tin → bot comment & gắn `needs/info` (auto-close sau N ngày).
- Không hoạt động → `stale` → lock.
