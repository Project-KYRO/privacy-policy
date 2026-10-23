---
layout: legal
title: "Garmin Connect API — Data Disclosure | KYRO"
description: "How KYRO (Movements Lab Co., Ltd.) collects, uses, processes, stores, and shares data obtained through the Garmin Connect API."
canonical: "https://project-kyro.github.io/privacy-policy/garmin.html"
---

# Garmin Connect API — Data Disclosure

_This page is part of the [KYRO Privacy Policy](./) and describes specifically how data obtained through the **Garmin Connect API** is collected, used, processed, stored, and shared. It is maintained by Movements Lab Co., Ltd. (주식회사 무브먼트랩, "the Company"), operator of the KYRO application._

**Last updated: 2026-06-17**

---

## 1. Scope

This disclosure applies only when a KYRO user explicitly connects their Garmin account to KYRO. Garmin data is never collected unless the user completes the Garmin OAuth authorization and grants consent. Users may disconnect at any time (see Section 7).

## 2. Data we collect via the Garmin Connect API

When a user authorizes the connection, the Company receives, through the Garmin Connect Activity API, the activity data the user has authorized, which may include:

- GPS route (latitude/longitude coordinates) and elevation
- Distance, pace, and duration
- Heart rate and cadence (including per-split values)
- Calories and step count
- Activity type, start time, and device/source information

The Company requests only the data scopes required to record and display a user's running activities. No Garmin data outside the user's authorized scope is collected.

## 3. How the data is used (purpose)

Garmin data is used solely to provide the user's own running experience within KYRO, identical to runs recorded natively in the app:

- Measuring, storing, and visualizing the user's own running records
- Computing splits, cumulative territory, rankings, and personal statistics
- Displaying the user's activity history to the user

Garmin data is **not** used for advertising, profiling, or any purpose unrelated to providing the running service the user requested.

## 4. How the data is processed

When Garmin sends a PING/PUSH webhook notification for a new or updated activity, the Company's backend (Cloudflare Workers) asynchronously retrieves the corresponding activity details and normalizes the track to compute splits and territory. Processing occurs only to deliver the features described in Section 3.

## 5. Where and how long the data is stored

- **Storage location:** Garmin-derived data is stored on **Supabase** (managed PostgreSQL database and object storage). Network processing and gateway functions are handled by **Cloudflare**. Both are contractual sub-processors acting solely under the Company's direction (see [Article 11 of the Privacy Policy](./#11-개인정보-처리-위탁)).
- **Encryption:** Data is encrypted at rest (AES-256) and in transit (TLS 1.3).
- **Retention:** Garmin-derived data is retained while the user's account is active and is **deleted without undue delay** when the user disconnects Garmin, is deregistered, or deletes their KYRO account (see Section 7).

## 6. Third-party sharing and AI services

The Company does **not** share, sell, transfer, or otherwise make available data obtained through the Garmin Connect API to:

- any third party, **including external AI providers, third-party AI services, or external data-processing services**, nor
- any party for purposes unrelated to providing the KYRO running service.

The sub-processors named in Section 5 (Supabase, Cloudflare) process Garmin data **only** to store and operate the service under the Company's direction and control, within the scope of their service agreements. This does not constitute third-party sharing, and these sub-processors are not "third-party AI services or external data-processing services" within the meaning of this disclosure.

## 7. User control — disconnect and deregistration

- A user may **disconnect** their Garmin account at any time from the KYRO app settings.
- Upon disconnection or **User Deregistration**, the Company stops collecting new Garmin data and deletes Garmin-derived data associated with the account without undue delay.
- Deleting the KYRO account also deletes all associated Garmin-derived data.

## 8. Contact

- Data Protection Officer: Ahn Jeongwoo (안정우)
- Email: support@kyro.team

For the full KYRO Privacy Policy, see <https://project-kyro.github.io/privacy-policy/>.

---

# Garmin Connect API — 데이터 처리 고지 (한국어)

_본 페이지는 [KYRO 개인정보처리방침](./)의 일부로서, **Garmin Connect API**를 통해 수집한 데이터를 어떻게 수집·이용·처리·저장·공유하는지를 구체적으로 설명합니다. KYRO 애플리케이션 운영사인 주식회사 무브먼트랩(이하 "회사")이 관리합니다._

**최종 업데이트: 2026-06-17**

## 1. 적용 범위

본 고지는 KYRO 회원이 본인의 Garmin 계정을 KYRO에 직접 연동한 경우에만 적용됩니다. 회원이 Garmin OAuth 인증을 완료하고 동의하지 않는 한 Garmin 데이터는 수집되지 않으며, 회원은 언제든지 연동을 해제할 수 있습니다(제7항).

## 2. Garmin Connect API를 통해 수집하는 데이터

회원이 연동에 동의하면, 회사는 Garmin Connect Activity API를 통해 회원이 허용한 활동 데이터를 수신하며, 다음을 포함할 수 있습니다.

- GPS 경로(위·경도 좌표) 및 고도
- 거리, 페이스, 시간
- 심박수 및 케이던스(구간별 값 포함)
- 칼로리 및 걸음 수
- 활동 유형, 시작 시각, 기기·소스 정보

회사는 러닝 활동의 기록·표시에 필요한 범위(scope)의 데이터만 요청하며, 회원이 허용한 범위 밖의 Garmin 데이터는 수집하지 않습니다.

## 3. 데이터의 이용 목적

Garmin 데이터는 앱 내에서 직접 기록한 러닝과 동일하게, 오로지 회원 본인의 러닝 경험 제공을 위해서만 이용됩니다.

- 회원 본인의 러닝 기록 측정·저장·시각화
- 구간(split)·누적 영토·랭킹·개인 통계 계산
- 회원 본인에게 활동 기록 표시

Garmin 데이터는 광고, 프로파일링, 또는 회원이 요청한 러닝 서비스 제공과 무관한 어떤 목적으로도 이용되지 않습니다.

## 4. 데이터의 처리 방식

Garmin이 신규·갱신 활동에 대한 PING/PUSH 웹훅 알림을 전송하면, 회사의 백엔드(Cloudflare Workers)가 비동기적으로 해당 활동 상세를 가져와 트랙을 정규화하여 구간·영토를 계산합니다. 처리는 제3항의 기능 제공을 위해서만 이루어집니다.

## 5. 데이터의 저장 위치 및 보유 기간

- **저장 위치:** Garmin 유래 데이터는 **Supabase**(관리형 PostgreSQL 및 객체 저장소)에 저장되며, 네트워크 처리·게이트웨이는 **Cloudflare**가 담당합니다. 양사는 회사의 지시·감독 하에서만 처리하는 계약상 수탁사입니다([처리방침 제11조](./#11-개인정보-처리-위탁) 참조).
- **암호화:** 저장 시 AES-256, 전송 시 TLS 1.3으로 암호화됩니다.
- **보유 기간:** Garmin 유래 데이터는 회원 자격이 유지되는 동안 보존되며, 회원이 Garmin 연동을 해제하거나 등록 해지(deregistration)되거나 KYRO 계정을 삭제하면 **지체 없이 파기**됩니다(제7항).

## 6. 제3자 공유 및 AI 서비스

회사는 Garmin Connect API를 통해 수집한 데이터를 다음 대상에 공유·판매·이전하거나 이용 가능하게 하지 **않습니다.**

- 외부 AI 제공업체, 제3자 AI 서비스, 외부 데이터 처리 서비스(external data-processing services)를 **포함한** 모든 제3자
- KYRO 러닝 서비스 제공과 무관한 목적의 어떤 당사자

제5항의 수탁사(Supabase, Cloudflare)는 서비스 계약 범위 내에서 회사의 지시·감독 하에 데이터를 저장·운영하기 위해서**만** Garmin 데이터를 처리합니다. 이는 제3자 제공에 해당하지 않으며, 해당 수탁사는 본 고지에서 말하는 "제3자 AI 서비스 또는 외부 데이터 처리 서비스"에 해당하지 않습니다.

## 7. 회원 통제 — 연동 해제 및 등록 해지

- 회원은 KYRO 앱 설정에서 언제든지 Garmin 계정 연동을 **해제**할 수 있습니다.
- 연동 해제 또는 **등록 해지(User Deregistration)** 시, 회사는 신규 Garmin 데이터 수집을 중단하고 해당 계정의 Garmin 유래 데이터를 지체 없이 파기합니다.
- KYRO 계정을 삭제하면 연계된 모든 Garmin 유래 데이터도 함께 삭제됩니다.

## 8. 문의

- 개인정보보호책임자: 안정우
- 이메일: support@kyro.team

전체 KYRO 개인정보처리방침은 <https://project-kyro.github.io/privacy-policy/>에서 확인할 수 있습니다.
