# Commit Archive Index

이 폴더는 git 커밋 219개를 커밋별 Markdown 파일로 정리한 아카이브다.

## 생성 기준
- 각 파일은 커밋 메타데이터, 변경 파일 목록, diff 통계, 원본 로그 요약을 포함한다.
- 해석과 의도 분석은 커밋 메시지와 변경 파일을 바탕으로 작성한 추정이며, 작성자의 직접 코멘트는 아니다.
- 파일명은 순번_짧은해시.md 형식으로 고정했다.

## 개발 단계 요약
- #1-6 그래프 백엔드 기초: txt2graph 기반 지식 그래프 생성과 Project ID 중심 상태 관리 API가 자리 잡으면서 초기 백엔드 골격이 형성된 구간이다.
- #7-33 시뮬레이션·리포트 백엔드 확장: OASIS 시뮬레이션, 프로필 생성, 로깅, 인터뷰, Report Agent, Zep 도구가 연결되며 분석 파이프라인이 크게 확장됐다.
- #34-75 프론트 워크플로 구축: 홈, 그래프 시각화, 메인 스텝 흐름, Step2/Step3 UI가 추가되며 제품형 프런트엔드가 빠르게 형성된 시기다.
- #76-113 리포트·대화 UX 고도화: Step4Report와 Step5Interaction이 반복적으로 다듬어지며 보고서 해석과 후속 대화 경험이 제품 형태로 정리됐다.
- #114-156 오픈소스 공개·운영 정비: 버전 선언, Docker 실험, 라이선스 조정, 다국어 README, Windows 호환성 보강 등 외부 공개와 운영 준비가 집중됐다.
- #157-180 히스토리 아카이브 도입: HistoryDatabase와 관련 API가 추가되며 과거 프로젝트와 결과를 탐색하는 홈 화면 흐름이 새로 생겼다.
- #181-219 안정화와 품질 개선: 환경설정, Docker 재도입, 인코딩, report_agent 프롬프트·렌더링, 그래프 페이징, reasoning model 예외 대응까지 안정화 작업이 이어졌다.

## 폴더 구조
- `01_graph_backend_basics/`: #001-006
- `02_simulation_report_backend/`: #007-033
- `03_frontend_workflow/`: #034-075
- `04_report_interaction_ux/`: #076-113
- `05_open_source_operations/`: #114-156
- `06_history_archive/`: #157-180
- `07_stabilization_quality/`: #181-219

## 관련 요약 문서
- [ROADMAP_FOR_PLANNING.md](./ROADMAP_FOR_PLANNING.md)
- [PM_MILESTONE_TABLE.md](./PM_MILESTONE_TABLE.md)
- [VIBE_CODING_GUIDE.md](./VIBE_CODING_GUIDE.md)

## 영역별 분포
- 문서/브랜딩: 70개
- 보고서 에이전트: 46개
- 시뮬레이션: 42개
- 그래프: 32개
- 배포/설정: 18개
- 백엔드 인프라: 8개
- 프로젝트 전반: 3개

## 커밋 목록
| 순번 | 해시 | 날짜 | 주요 영역 | 제목 |
| --- | --- | --- | --- | --- |
| 001 | 38e3d05 | 2025-11-26 | 프로젝트 전반 | [Initial commit](./01_graph_backend_basics/001_38e3d05.md) |
| 002 | 9657061 | 2025-11-28 | 그래프 | [Add initial implementation of txt2graph tool for knowledge graph generation](./01_graph_backend_basics/002_9657061.md) |
| 003 | 08f417f | 2025-11-28 | 백엔드 인프라 | [Introduce Project ID for context management, finalizing the stateful API pipeline from file submission to graph construction.](./01_graph_backend_basics/003_08f417f.md) |
| 004 | 3156f94 | 2025-11-28 | 그래프 | [Remove deprecated files and modules from the txt2graph tool, including the main application, graph builder, text extractor, and associated resources. This cleanup streamlines the project structure and prepares for future enhancements.](./01_graph_backend_basics/004_3156f94.md) |
| 005 | e98da6b | 2025-11-28 | 백엔드 인프라 | [Enhance backend startup logging and API endpoint display](./01_graph_backend_basics/005_e98da6b.md) |
| 006 | c60e6e1 | 2025-11-29 | 그래프 | [Refactor project creation process in API documentation and code](./01_graph_backend_basics/006_c60e6e1.md) |
| 007 | 5f159f6 | 2025-12-01 | 시뮬레이션 | [Enhance backend functionality with OASIS simulation features](./02_simulation_report_backend/007_5f159f6.md) |
| 008 | af5c235 | 2025-12-01 | 시뮬레이션 | [Enhance OASIS simulation capabilities and profile generation](./02_simulation_report_backend/008_af5c235.md) |
| 009 | 3cc5e3f | 2025-12-02 | 시뮬레이션 | [Refactor simulation management and enhance logging capabilities](./02_simulation_report_backend/009_3cc5e3f.md) |
| 010 | d4fac63 | 2025-12-02 | 백엔드 인프라 | [Enhance simulation management and logging features](./02_simulation_report_backend/010_d4fac63.md) |
| 011 | 2333121 | 2025-12-02 | 문서/브랜딩 | [Update README.md for MiroFish Backend with detailed technical documentation](./02_simulation_report_backend/011_2333121.md) |
| 012 | 2df3104 | 2025-12-04 | 프로젝트 전반 | [Add balance check script for OpenRouter API](./02_simulation_report_backend/012_2df3104.md) |
| 013 | 0302b8f | 2025-12-04 | 시뮬레이션 | [Add MaxTokensWarningFilter to logging and set semaphore for LLM requests](./02_simulation_report_backend/013_0302b8f.md) |
| 014 | 39253b3 | 2025-12-04 | 배포/설정 | [Update .env.example and enhance create_model function for dual LLM configuration](./02_simulation_report_backend/014_39253b3.md) |
| 015 | 88676e8 | 2025-12-04 | 시뮬레이션 | [Implement real-time profile retrieval and saving in simulation API](./02_simulation_report_backend/015_88676e8.md) |
| 016 | 3c1d554 | 2025-12-04 | 시뮬레이션 | [Add function to retrieve agent names from configuration](./02_simulation_report_backend/016_3c1d554.md) |
| 017 | 5b4f02f | 2025-12-05 | 배포/설정 | [Enhance simulation configuration and management features](./02_simulation_report_backend/017_5b4f02f.md) |
| 018 | e4761da | 2025-12-05 | 시뮬레이션 | [Enhance action logging in simulation scripts](./02_simulation_report_backend/018_e4761da.md) |
| 019 | e3768e2 | 2025-12-05 | 그래프 | [Implement dynamic graph memory update feature for simulations](./02_simulation_report_backend/019_e3768e2.md) |
| 020 | e9b49e3 | 2025-12-05 | 그래프 | [Refactor activity logging and update Zep integration for real-time processing](./02_simulation_report_backend/020_e9b49e3.md) |
| 021 | 29bff9c | 2025-12-05 | 그래프 | [Refactor content handling in activity logging and simulation scripts](./02_simulation_report_backend/021_29bff9c.md) |
| 022 | 1042d50 | 2025-12-08 | 시뮬레이션 | [Implement Interview feature for agent interactions in simulations](./02_simulation_report_backend/022_1042d50.md) |
| 023 | 1f191cb | 2025-12-08 | 시뮬레이션 | [Enhance interview prompt handling and update README.md](./02_simulation_report_backend/023_1f191cb.md) |
| 024 | 3f750ff | 2025-12-08 | 그래프 | [Enhance action context enrichment and update activity logging](./02_simulation_report_backend/024_3f750ff.md) |
| 025 | 91eb73a | 2025-12-09 | 그래프 | [Enhance signal handling and suppress warnings in simulation scripts](./02_simulation_report_backend/025_91eb73a.md) |
| 026 | 78230b7 | 2025-12-09 | 백엔드 인프라 | [Remove warnings suppression for multiprocessing in run scripts](./02_simulation_report_backend/026_78230b7.md) |
| 027 | 8d63f40 | 2025-12-09 | 백엔드 인프라 | [Remove startup message logging from the Flask application in `run.py` to streamline output during server initialization. This change simplifies the code and reduces unnecessary console output, particularly in debug mode.](./02_simulation_report_backend/027_8d63f40.md) |
| 028 | 5ece3f6 | 2025-12-09 | 보고서 에이전트 | [Implement Report Agent for automated report generation and interaction](./02_simulation_report_backend/028_5ece3f6.md) |
| 029 | a0c97b1 | 2025-12-09 | 그래프 | [Enhance Report Agent and Zep Tools with new search functionalities](./02_simulation_report_backend/029_a0c97b1.md) |
| 030 | b022c38 | 2025-12-09 | 그래프 | [Add interview functionality to Report Agent and Zep Tools](./02_simulation_report_backend/030_b022c38.md) |
| 031 | 74aab44 | 2025-12-09 | 그래프 | [Enhance interview functionality in Report Agent and Zep Tools](./02_simulation_report_backend/031_74aab44.md) |
| 032 | 5396b21 | 2025-12-09 | 시뮬레이션 | [Remove obsolete simulation files and configurations](./02_simulation_report_backend/032_5396b21.md) |
| 033 | ed8bfec | 2025-12-09 | 프로젝트 전반 | [Remove unused balance check script for OpenRouter API](./02_simulation_report_backend/033_ed8bfec.md) |
| 034 | d59bda9 | 2025-12-10 | 문서/브랜딩 | [Add MiroFish logo images](./03_frontend_workflow/034_d59bda9.md) |
| 035 | b67e14c | 2025-12-10 | 문서/브랜딩 | [Add project status report and frontend documentation](./03_frontend_workflow/035_b67e14c.md) |
| 036 | 6226cba | 2025-12-10 | 문서/브랜딩 | [Enhance homepage layout and styling](./03_frontend_workflow/036_6226cba.md) |
| 037 | 81b3fb3 | 2025-12-10 | 문서/브랜딩 | [Revamp homepage content and styling](./03_frontend_workflow/037_81b3fb3.md) |
| 038 | 81e2f3d | 2025-12-10 | 문서/브랜딩 | [Implement scroll functionality and enhance button styling in Home.vue](./03_frontend_workflow/038_81e2f3d.md) |
| 039 | d4dd4b3 | 2025-12-10 | 문서/브랜딩 | [Revise Home.vue content and layout for enhanced clarity and engagement](./03_frontend_workflow/039_d4dd4b3.md) |
| 040 | 5a27b7c | 2025-12-10 | 그래프 | [Add D3.js dependency and implement pending upload state management](./03_frontend_workflow/040_5a27b7c.md) |
| 041 | 23927dc | 2025-12-10 | 그래프 | [Enhance graph visualization and data polling in Process.vue](./03_frontend_workflow/041_23927dc.md) |
| 042 | b7db395 | 2025-12-10 | 그래프 | [Enhance graph data handling and user interaction in Process.vue](./03_frontend_workflow/042_b7db395.md) |
| 043 | 8565f04 | 2025-12-10 | 그래프 | [Add detailed node and edge information panel in Process.vue](./03_frontend_workflow/043_8565f04.md) |
| 044 | a90b683 | 2025-12-10 | 그래프 | [Enhance graph data retrieval and detail display in Process.vue and graph_builder.py](./03_frontend_workflow/044_a90b683.md) |
| 045 | a661046 | 2025-12-10 | 그래프 | [Refactor Process.vue layout and enhance full-screen functionality](./03_frontend_workflow/045_a661046.md) |
| 046 | 35da38e | 2025-12-11 | 그래프 | [Add GraphPanel and WorkbenchPanel components for enhanced visualization and interaction](./03_frontend_workflow/046_35da38e.md) |
| 047 | 573e453 | 2025-12-11 | 그래프 | [Enhance GraphPanel.vue with detailed node and edge information display](./03_frontend_workflow/047_573e453.md) |
| 048 | 1f6f79c | 2025-12-11 | 그래프 | [Add gravitational forces to node simulation in GraphPanel.vue](./03_frontend_workflow/048_1f6f79c.md) |
| 049 | ba6f63f | 2025-12-11 | 문서/브랜딩 | [Enhance MainView.vue with workflow step indicators and improved styling](./03_frontend_workflow/049_ba6f63f.md) |
| 050 | 860677b | 2025-12-11 | 그래프 | [Update GraphPanel.vue and WorkbenchPanel.vue for improved UI and clarity](./03_frontend_workflow/050_860677b.md) |
| 051 | fc95cc6 | 2025-12-11 | 그래프 | [Add simulation API and environment setup components](./03_frontend_workflow/051_fc95cc6.md) |
| 052 | 01d94f3 | 2025-12-11 | 그래프 | [Update simulation components and descriptions for clarity and functionality](./03_frontend_workflow/052_01d94f3.md) |
| 053 | 734b6a9 | 2025-12-11 | 시뮬레이션 | [Refactor Step2EnvSetup.vue for improved profile display and statistics](./03_frontend_workflow/053_734b6a9.md) |
| 054 | 11e5646 | 2025-12-11 | 시뮬레이션 | [Refactor Step2EnvSetup.vue for enhanced profile details and layout](./03_frontend_workflow/054_11e5646.md) |
| 055 | ceb1399 | 2025-12-11 | 시뮬레이션 | [Update Step2EnvSetup.vue for improved clarity in simulation configuration](./03_frontend_workflow/055_ceb1399.md) |
| 056 | 8b5d082 | 2025-12-11 | 시뮬레이션 | [Add real-time simulation configuration endpoint and update frontend components](./03_frontend_workflow/056_8b5d082.md) |
| 057 | c44cb13 | 2025-12-11 | 시뮬레이션 | [Refactor Step2EnvSetup.vue for improved hot topics display and timeline styling](./03_frontend_workflow/057_c44cb13.md) |
| 058 | 39824c8 | 2025-12-11 | 시뮬레이션 | [Enhance Step2EnvSetup.vue with agent username display and styling improvements](./03_frontend_workflow/058_39824c8.md) |
| 059 | 2812225 | 2025-12-11 | 시뮬레이션 | [Revamp Step2EnvSetup.vue styling for improved user experience](./03_frontend_workflow/059_2812225.md) |
| 060 | 9ac6303 | 2025-12-11 | 시뮬레이션 | [Enhance Step2EnvSetup.vue with detailed configuration display and improved styling](./03_frontend_workflow/060_9ac6303.md) |
| 061 | 5c6a569 | 2025-12-11 | 시뮬레이션 | [Refactor Step2EnvSetup.vue for improved configuration clarity and styling](./03_frontend_workflow/061_5c6a569.md) |
| 062 | fdbb0e2 | 2025-12-11 | 그래프 | [Update Step1GraphBuild.vue and Step2EnvSetup.vue with API endpoint notes and enhanced styling](./03_frontend_workflow/062_fdbb0e2.md) |
| 063 | 65c1835 | 2025-12-12 | 시뮬레이션 | [Enhance Step2EnvSetup.vue with modal transition effects for improved user experience](./03_frontend_workflow/063_65c1835.md) |
| 064 | bf7fe8b | 2025-12-12 | 시뮬레이션 | [Revamp simulation rounds configuration in Step2EnvSetup.vue for enhanced user experience](./03_frontend_workflow/064_bf7fe8b.md) |
| 065 | c287fe7 | 2025-12-12 | 시뮬레이션 | [Remove unnecessary whitespace at the end of Step2EnvSetup.vue for cleaner code.](./03_frontend_workflow/065_c287fe7.md) |
| 066 | 4345f30 | 2025-12-12 | 시뮬레이션 | [Enhance simulation preparation process and frontend display for improved user experience](./03_frontend_workflow/066_4345f30.md) |
| 067 | aad01f0 | 2025-12-12 | 시뮬레이션 | [Enhance logging and progress display in Step2EnvSetup.vue for improved user experience](./03_frontend_workflow/067_aad01f0.md) |
| 068 | f8a5881 | 2025-12-12 | 시뮬레이션 | [Enhance simulation functionality and frontend components for improved user experience](./03_frontend_workflow/068_f8a5881.md) |
| 069 | 0577ecd | 2025-12-12 | 시뮬레이션 | [Add new JSON data file and enhance simulation management features](./03_frontend_workflow/069_0577ecd.md) |
| 070 | ec418c1 | 2025-12-12 | 시뮬레이션 | [Implement simulation environment management features in frontend](./03_frontend_workflow/070_ec418c1.md) |
| 071 | d768fd1 | 2025-12-12 | 시뮬레이션 | [Enhance simulation file management and frontend status display](./03_frontend_workflow/071_d768fd1.md) |
| 072 | c91dad3 | 2025-12-12 | 시뮬레이션 | [Enhance Step3Simulation component with detailed action tracking and UI improvements](./03_frontend_workflow/072_c91dad3.md) |
| 073 | f590784 | 2025-12-12 | 시뮬레이션 | [Enhance Step3Simulation and Step2EnvSetup components for improved clarity and user experience](./03_frontend_workflow/073_f590784.md) |
| 074 | 307990d | 2025-12-12 | 시뮬레이션 | [Update profile display logic in Step2EnvSetup and modal components for consistency](./03_frontend_workflow/074_307990d.md) |
| 075 | 2fd1227 | 2025-12-12 | 시뮬레이션 | [Enhance Step3Simulation component with dynamic graph memory update feature](./03_frontend_workflow/075_2fd1227.md) |
| 076 | 8949ae6 | 2025-12-13 | 그래프 | [Enhance report generation process with improved formatting and content management](./04_report_interaction_ux/076_8949ae6.md) |
| 077 | b4435e2 | 2025-12-13 | 그래프 | [Add report ID generation and logging features for report generation process](./04_report_interaction_ux/077_b4435e2.md) |
| 078 | f904407 | 2025-12-13 | 보고서 에이전트 | [Implement report generation features and UI enhancements](./04_report_interaction_ux/078_f904407.md) |
| 079 | 851b12d | 2025-12-13 | 보고서 에이전트 | [Adjust max-height of report display in Step4Report component for improved visibility](./04_report_interaction_ux/079_851b12d.md) |
| 080 | fde7972 | 2025-12-14 | 그래프 | [Enhance agent bio display and tool result presentation in Step4Report component](./04_report_interaction_ux/080_fde7972.md) |
| 081 | 9be2c28 | 2025-12-14 | 보고서 에이전트 | [Refactor report logging and enhance report generation features](./04_report_interaction_ux/081_9be2c28.md) |
| 082 | 1db72dc | 2025-12-14 | 보고서 에이전트 | [Remove status bar from Step4Report component to streamline UI and improve layout. This change simplifies the report display by eliminating unnecessary elements, enhancing user experience and focus on content.](./04_report_interaction_ux/082_1db72dc.md) |
| 083 | be90a46 | 2025-12-14 | 보고서 에이전트 | [Add custom scrollbar styles for left and right panels in Step4Report component](./04_report_interaction_ux/083_be90a46.md) |
| 084 | 2215c47 | 2025-12-14 | 보고서 에이전트 | [Refactor Step4Report component styles for improved transitions and layout](./04_report_interaction_ux/084_2215c47.md) |
| 085 | a097de4 | 2025-12-14 | 그래프 | [Enhance text output formatting and remove truncation in zep_tools.py](./04_report_interaction_ux/085_a097de4.md) |
| 086 | 0fa2363 | 2025-12-14 | 보고서 에이전트 | [Update maximum limits for tool calls and iterations in ReportAgent class](./04_report_interaction_ux/086_0fa2363.md) |
| 087 | b8817aa | 2025-12-15 | 보고서 에이전트 | [Enhance Step4Report component with detailed interview parsing and improved display](./04_report_interaction_ux/087_b8817aa.md) |
| 088 | ab8b116 | 2025-12-15 | 시뮬레이션 | [Update height in Step3Simulation and Step4Report components for improved layout consistency](./04_report_interaction_ux/088_ab8b116.md) |
| 089 | c6d26fc | 2025-12-16 | 보고서 에이전트 | [Refactor Step4Report component to implement Q&A format for interview display](./04_report_interaction_ux/089_c6d26fc.md) |
| 090 | 2247d3d | 2025-12-16 | 보고서 에이전트 | [Refactor Step4Report component for improved layout and user experience](./04_report_interaction_ux/090_2247d3d.md) |
| 091 | 0f6395b | 2025-12-16 | 보고서 에이전트 | [Update Step4Report component header and padding for improved clarity and layout](./04_report_interaction_ux/091_0f6395b.md) |
| 092 | 4385f17 | 2025-12-16 | 보고서 에이전트 | [Update Step4Report component for improved localization and scrollbar styling](./04_report_interaction_ux/092_4385f17.md) |
| 093 | 705bebe | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with workflow overview and improved styling](./04_report_interaction_ux/093_705bebe.md) |
| 094 | daae471 | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with tool-specific icons and improved action buttons](./04_report_interaction_ux/094_daae471.md) |
| 095 | 5f22835 | 2025-12-16 | 보고서 에이전트 | [Refactor Step4Report component for enhanced workflow display and loading states](./04_report_interaction_ux/095_5f22835.md) |
| 096 | 1659665 | 2025-12-16 | 보고서 에이전트 | [Refactor interview parsing and answer splitting logic in Step4Report component](./04_report_interaction_ux/096_1659665.md) |
| 097 | c811f45 | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with individual selection reason parsing and display](./04_report_interaction_ux/097_c811f45.md) |
| 098 | 6bf1f29 | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with comprehensive data parsing and improved display](./04_report_interaction_ux/098_6bf1f29.md) |
| 099 | e3b82e6 | 2025-12-16 | 보고서 에이전트 | [Refactor Step4Report component to remove tab icons for a cleaner interface](./04_report_interaction_ux/099_e3b82e6.md) |
| 100 | 3b20672 | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with improved result display and layout adjustments](./04_report_interaction_ux/100_3b20672.md) |
| 101 | 70922a3 | 2025-12-16 | 보고서 에이전트 | [Implement interaction features in Step5Interaction component and add routing for interaction view](./04_report_interaction_ux/101_70922a3.md) |
| 102 | cb47e98 | 2025-12-16 | 보고서 에이전트 | [Update ReportAgent to enhance report retrieval and streamline tool call process](./04_report_interaction_ux/102_cb47e98.md) |
| 103 | c738d7e | 2025-12-16 | 보고서 에이전트 | [Refactor Step5Interaction component to enhance user interaction and UI elements](./04_report_interaction_ux/103_c738d7e.md) |
| 104 | 318d60f | 2025-12-16 | 보고서 에이전트 | [Refactor Step5Interaction component to streamline profile display and remove unused topics section](./04_report_interaction_ux/104_318d60f.md) |
| 105 | c43b83f | 2025-12-16 | 보고서 에이전트 | [Enhance Step5Interaction component with professional design updates and improved UI elements](./04_report_interaction_ux/105_c43b83f.md) |
| 106 | 4bd3c85 | 2025-12-16 | 보고서 에이전트 | [Enhance Step5Interaction component with updated UI elements and improved functionality](./04_report_interaction_ux/106_4bd3c85.md) |
| 107 | 78c8c43 | 2025-12-16 | 보고서 에이전트 | [Add Report Agent Tools Card to Step5Interaction component](./04_report_interaction_ux/107_78c8c43.md) |
| 108 | cc094e4 | 2025-12-16 | 보고서 에이전트 | [Implement chat history caching and enhance message rendering in Step5Interaction component](./04_report_interaction_ux/108_cc094e4.md) |
| 109 | 9db7781 | 2025-12-16 | 보고서 에이전트 | [Enhance Step5Interaction component with improved tool description and memory feature](./04_report_interaction_ux/109_9db7781.md) |
| 110 | d096aa2 | 2025-12-16 | 문서/브랜딩 | [Remove outdated README.md and update favicon in index.html](./04_report_interaction_ux/110_d096aa2.md) |
| 111 | efc7fbc | 2025-12-16 | 보고서 에이전트 | [Enhance Step5Interaction component to improve response handling and survey result processing](./04_report_interaction_ux/111_efc7fbc.md) |
| 112 | 99c1b19 | 2025-12-16 | 보고서 에이전트 | [Update ReportAgent to reduce maximum tool calls and iterations for improved efficiency](./04_report_interaction_ux/112_99c1b19.md) |
| 113 | e2b1a15 | 2025-12-16 | 보고서 에이전트 | [Enhance Step4Report component with section numbering and improved scroll behavior](./04_report_interaction_ux/113_e2b1a15.md) |
| 114 | e432e22 | 2025-12-17 | 배포/설정 | [Update project configuration and structure with Docker support and environment variable adjustments](./05_open_source_operations/114_e432e22.md) |
| 115 | 08688a8 | 2025-12-17 | 배포/설정 | [Update project setup scripts and enhance README for clarity](./05_open_source_operations/115_08688a8.md) |
| 116 | 9291635 | 2025-12-17 | 배포/설정 | [Add Apache License 2.0 to the project](./05_open_source_operations/116_9291635.md) |
| 117 | 97a6494 | 2025-12-17 | 배포/설정 | [Update project license to Apache-2.0 in package.json, README.md, and pyproject.toml](./05_open_source_operations/117_97a6494.md) |
| 118 | 136843a | 2025-12-18 | 배포/설정 | [Initialize project with version 0.1.0 and update package configurations](./05_open_source_operations/118_136843a.md) |
| 119 | a47eb1e | 2025-12-19 | 배포/설정 | [Refactor project structure by removing Docker support and updating environment configuration](./05_open_source_operations/119_a47eb1e.md) |
| 120 | 5a67cd3 | 2025-12-19 | 문서/브랜딩 | [Update README.md to adjust logo display size for improved responsiveness](./05_open_source_operations/120_5a67cd3.md) |
| 121 | 2c39856 | 2025-12-19 | 문서/브랜딩 | [Resize logo image to 70% width in README](./05_open_source_operations/121_2c39856.md) |
| 122 | 43d80c5 | 2025-12-19 | 문서/브랜딩 | [Increase logo width in README](./05_open_source_operations/122_43d80c5.md) |
| 123 | d787ebc | 2025-12-19 | 문서/브랜딩 | [Add English README file for MiroFish project](./05_open_source_operations/123_d787ebc.md) |
| 124 | 4ddbb9d | 2025-12-19 | 문서/브랜딩 | [Update README files to remove strong tag and add line break for improved formatting](./05_open_source_operations/124_4ddbb9d.md) |
| 125 | fb3b412 | 2025-12-19 | 문서/브랜딩 | [Update README](./05_open_source_operations/125_fb3b412.md) |
| 126 | abd4656 | 2025-12-19 | 배포/설정 | [Remove file](./05_open_source_operations/126_abd4656.md) |
| 127 | e5dbeb2 | 2025-12-19 | 배포/설정 | [Add GNU AGPL v3 License](./05_open_source_operations/127_e5dbeb2.md) |
| 128 | f342eaf | 2025-12-19 | 시뮬레이션 | [Update README files to enhance vision section and add acknowledgments for OASIS framework](./05_open_source_operations/128_f342eaf.md) |
| 129 | 9d09a34 | 2025-12-19 | 문서/브랜딩 | [Update Home.vue to remove trailing punctuation in hero description for improved readability](./05_open_source_operations/129_9d09a34.md) |
| 130 | 593f705 | 2025-12-19 | 문서/브랜딩 | [Update README files to clarify the description of the Python package manager by removing the reference to pip as an alternative.](./05_open_source_operations/130_593f705.md) |
| 131 | e749931 | 2025-12-19 | 그래프 | [Enhance README files by correcting phrasing in the vision section and adding a detailed workflow section outlining the steps for graph building, environment setup, simulation, report generation, and deep interaction.](./05_open_source_operations/131_e749931.md) |
| 132 | ed2208f | 2025-12-21 | 문서/브랜딩 | [Remove frontend README.md file as part of project restructuring.](./05_open_source_operations/132_ed2208f.md) |
| 133 | fb9a3e5 | 2025-12-22 | 문서/브랜딩 | [Update README.](./05_open_source_operations/133_fb9a3e5.md) |
| 134 | 4e96019 | 2025-12-22 | 배포/설정 | [Change project license from Apache-2.0 to AGPL-3.0 in package.json, package-lock.json, and backend/pyproject.toml.](./05_open_source_operations/134_4e96019.md) |
| 135 | 61f1ee7 | 2025-12-22 | 문서/브랜딩 | [Update README files to include demo video links and enhance content presentation, along with adding a new demo video image.](./05_open_source_operations/135_61f1ee7.md) |
| 136 | b669184 | 2025-12-22 | 문서/브랜딩 | [Update README files to replace demo video link with a direct URL for improved accessibility.](./05_open_source_operations/136_b669184.md) |
| 137 | 29a95b0 | 2025-12-22 | 문서/브랜딩 | [Add GitHub badges and version information to README files for better visibility and project tracking.](./05_open_source_operations/137_29a95b0.md) |
| 138 | e3b6a79 | 2025-12-23 | 문서/브랜딩 | [Add note about MiroFish's development environment in README files for clarity on Windows compatibility.](./05_open_source_operations/138_e3b6a79.md) |
| 139 | e849183 | 2025-12-23 | 문서/브랜딩 | [Update Home.vue to change GitHub link to the correct repository URL for accurate navigation.](./05_open_source_operations/139_e849183.md) |
| 140 | 84113ce | 2025-12-23 | 문서/브랜딩 | [Update README files to open demo video link in a new tab for improved user experience.](./05_open_source_operations/140_84113ce.md) |
| 141 | 9b231d3 | 2025-12-23 | 문서/브랜딩 | [Enhance README with project statistics section](./05_open_source_operations/141_9b231d3.md) |
| 142 | 39ba5b1 | 2025-12-23 | 문서/브랜딩 | [Update README-EN.md to add project statistics section and ensure proper formatting](./05_open_source_operations/142_39ba5b1.md) |
| 143 | 84f9fb7 | 2025-12-23 | 문서/브랜딩 | [Update video link description in README.md](./05_open_source_operations/143_84f9fb7.md) |
| 144 | 96b151c | 2025-12-23 | 문서/브랜딩 | [Update README-EN.md to clarify demo video link description for better user engagement](./05_open_source_operations/144_96b151c.md) |
| 145 | 4d24236 | 2025-12-24 | 문서/브랜딩 | [Add Shanda Group logo and acknowledgment in README files for strategic support](./05_open_source_operations/145_4d24236.md) |
| 146 | abf2ba6 | 2025-12-24 | 문서/브랜딩 | [Update README](./05_open_source_operations/146_abf2ba6.md) |
| 147 | 44424f2 | 2025-12-26 | 시뮬레이션 | [Update font styles across the application to include 'Noto Sans SC' for improved typography consistency.](./05_open_source_operations/147_44424f2.md) |
| 148 | 1987f53 | 2025-12-26 | 문서/브랜딩 | [Update font weights in Home.vue for improved visual hierarchy and consistency.](./05_open_source_operations/148_1987f53.md) |
| 149 | f46c1a9 | 2025-12-26 | 백엔드 인프라 | [Add UTF-8 encoding support for Windows console in run.py and logger.py to prevent character encoding issues](./05_open_source_operations/149_f46c1a9.md) |
| 150 | 067855f | 2025-12-26 | 시뮬레이션 | [Add UTF-8 encoding support for Windows in simulation_runner.py and run_parallel_simulation.py to resolve character encoding issues with third-party libraries.](./05_open_source_operations/150_067855f.md) |
| 151 | 8bd7687 | 2025-12-30 | 시뮬레이션 | [Add SIGHUP signal handling in SimulationRunner for Unix systems](./05_open_source_operations/151_8bd7687.md) |
| 152 | 4be144c | 2025-12-30 | 배포/설정 | [Refactor process termination in SimulationRunner to support cross-platform handling and improve code clarity. Update development script to ensure concurrent processes are terminated correctly.](./05_open_source_operations/152_4be144c.md) |
| 153 | 84dd2cb | 2025-12-30 | 배포/설정 | [Fix: Change backend dev color to green](./05_open_source_operations/153_84dd2cb.md) |
| 154 | c0aa078 | 2025-12-30 | 배포/설정 | [Merge pull request #12 from 666ghj/cursor/backend-terminal-color-change-14fd](./05_open_source_operations/154_c0aa078.md) |
| 155 | fa7ab33 | 2025-12-30 | 문서/브랜딩 | [Add Ask DeepWiki badge to README files for enhanced visibility and user engagement.](./05_open_source_operations/155_fa7ab33.md) |
| 156 | 8b80603 | 2025-12-30 | 문서/브랜딩 | [Update README.](./05_open_source_operations/156_8b80603.md) |
| 157 | e6da45e | 2025-12-31 | 문서/브랜딩 | [feat(history): 添加首页历史项目展示组件](./06_history_archive/157_e6da45e.md) |
| 158 | 2acdd73 | 2025-12-31 | 문서/브랜딩 | [style(HistoryDatabase): update grid background size and opacity for improved aesthetics](./06_history_archive/158_2acdd73.md) |
| 159 | 6fc0a0d | 2025-12-31 | 문서/브랜딩 | [refactor(HistoryDatabase): simplify CTA button positioning and adjust layout for improved responsiveness](./06_history_archive/159_6fc0a0d.md) |
| 160 | 9d5fad8 | 2026-01-07 | 문서/브랜딩 | [Update README.](./06_history_archive/160_9d5fad8.md) |
| 161 | 992f7d1 | 2026-01-07 | 시뮬레이션 | [refactor(simulation): enhance simulation data retrieval and project file handling](./06_history_archive/161_992f7d1.md) |
| 162 | d90ec77 | 2026-01-07 | 문서/브랜딩 | [translate(HistoryDatabase): change section title from English to Chinese](./06_history_archive/162_d90ec77.md) |
| 163 | dfab81a | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): optimize card expansion behavior with debounce and animation lock](./06_history_archive/163_dfab81a.md) |
| 164 | d7169ba | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): dynamically calculate container height based on card expansion state](./06_history_archive/164_d7169ba.md) |
| 165 | f32f571 | 2026-01-09 | 문서/브랜딩 | [style(HistoryDatabase): adjust grid background position for improved layout](./06_history_archive/165_f32f571.md) |
| 166 | 5a0c705 | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): enhance card expansion logic with pending state management](./06_history_archive/166_5a0c705.md) |
| 167 | cdf1373 | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): update card display to show round progress and time](./06_history_archive/167_cdf1373.md) |
| 168 | 5e865c0 | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): improve project display logic and loading states](./06_history_archive/168_5e865c0.md) |
| 169 | d79ea2b | 2026-01-09 | 문서/브랜딩 | [refactor(HistoryDatabase): enhance loading logic and card positioning](./06_history_archive/169_d79ea2b.md) |
| 170 | aa47087 | 2026-01-09 | 문서/브랜딩 | [style(HistoryDatabase): adjust padding and max-width for improved layout](./06_history_archive/170_aa47087.md) |
| 171 | b4fe7f2 | 2026-01-09 | 문서/브랜딩 | [feat(HistoryDatabase): add project detail modal for enhanced user interaction](./06_history_archive/171_b4fe7f2.md) |
| 172 | e25d2e3 | 2026-01-09 | 시뮬레이션 | [feat(SimulationAPI): add function to retrieve latest report ID for a given simulation](./06_history_archive/172_e25d2e3.md) |
| 173 | 0742194 | 2026-01-09 | 문서/브랜딩 | [style(HistoryDatabase): enhance modal design and transition effects](./06_history_archive/173_0742194.md) |
| 174 | 4977324 | 2026-01-09 | 문서/브랜딩 | [style(HistoryDatabase): enhance card header and footer layout with status icons](./06_history_archive/174_4977324.md) |
| 175 | cf4b358 | 2026-01-09 | 문서/브랜딩 | [docs(README): update Python version requirements and enhance contact section](./06_history_archive/175_cf4b358.md) |
| 176 | 8c81712 | 2026-01-09 | 문서/브랜딩 | [style(HistoryDatabase): update modal layout and enhance user guidance](./06_history_archive/176_8c81712.md) |
| 177 | 416eb6c | 2026-01-09 | 문서/브랜딩 | [Update README](./06_history_archive/177_416eb6c.md) |
| 178 | 08b2e78 | 2026-01-09 | 문서/브랜딩 | [Update README](./06_history_archive/178_08b2e78.md) |
| 179 | 11d3928 | 2026-01-09 | 문서/브랜딩 | [Update README](./06_history_archive/179_11d3928.md) |
| 180 | 9668ab4 | 2026-01-09 | 문서/브랜딩 | [Update README.md](./06_history_archive/180_9668ab4.md) |
| 181 | ede4106 | 2026-01-14 | 문서/브랜딩 | [fix(Home.vue): update version text from V1.0 to v0.1 for accuracy](./07_stabilization_quality/181_ede4106.md) |
| 182 | ca24ee0 | 2026-01-15 | 배포/설정 | [chore(env.example): update LLM model configuration and clarify boost settings.](./07_stabilization_quality/182_ca24ee0.md) |
| 183 | 56b8bab | 2026-01-16 | 그래프 | [feat(ZepGraphMemoryUpdater): add platform display name mapping and logging enhancements.](./07_stabilization_quality/183_56b8bab.md) |
| 184 | 8898c57 | 2026-01-16 | 문서/브랜딩 | [chore(Screenshot): update binary image file for improved visual content.](./07_stabilization_quality/184_8898c57.md) |
| 185 | 3c89f39 | 2026-01-16 | 문서/브랜딩 | [chore(Screenshot): replace binary image file to enhance visual quality.](./07_stabilization_quality/185_3c89f39.md) |
| 186 | 49847c5 | 2026-01-16 | 보고서 에이전트 | [feat(Step5Interaction): add section number display for improved user navigation](./07_stabilization_quality/186_49847c5.md) |
| 187 | 085aa6b | 2026-01-18 | 그래프 | [fix(GraphPanel): optimize force graph drag behavior to prevent simulation restart on click](./07_stabilization_quality/187_085aa6b.md) |
| 188 | 57e7225 | 2026-01-18 | 문서/브랜딩 | [chore(README): remove note about Windows compatibility from prerequisites section.](./07_stabilization_quality/188_57e7225.md) |
| 189 | be2acf6 | 2026-01-20 | 시뮬레이션 | [feat(README): add demo video sections for Wuhan University Public Opinion and Dream of the Red Chamber simulations; include new image asset](./07_stabilization_quality/189_be2acf6.md) |
| 190 | fa19242 | 2026-01-20 | 문서/브랜딩 | [fix(README): update image asset for Dream of the Red Chamber demo video section](./07_stabilization_quality/190_fa19242.md) |
| 191 | 824e81e | 2026-01-20 | 문서/브랜딩 | [refactor(README): update demo video section titles for clarity and consistency](./07_stabilization_quality/191_824e81e.md) |
| 192 | b0e065e | 2026-01-20 | 문서/브랜딩 | [refactor(README): update demo video section to include new financial and political prediction examples](./07_stabilization_quality/192_b0e065e.md) |
| 193 | 94633e1 | 2026-01-20 | 문서/브랜딩 | [refactor(README): update demo video section titles and clarify LLM API configuration instructions](./07_stabilization_quality/193_94633e1.md) |
| 194 | 9556854 | 2026-01-20 | 배포/설정 | [refactor(.env.example): update LLM API configuration comments for clarity and add usage note](./07_stabilization_quality/194_9556854.md) |
| 195 | 0efd935 | 2026-01-22 | 배포/설정 | [feat(docker): add Docker support with Dockerfile, docker-compose.yml, and .dockerignore; update README for Docker deployment instructions](./07_stabilization_quality/195_0efd935.md) |
| 196 | 390c120 | 2026-01-22 | 백엔드 인프라 | [fix(file_parser): handle non-UTF-8 encoded text files with automatic encoding detection](./07_stabilization_quality/196_390c120.md) |
| 197 | 93e1a59 | 2026-01-22 | 문서/브랜딩 | [feat(README): add Docker badge to README files for enhanced visibility of Docker support](./07_stabilization_quality/197_93e1a59.md) |
| 198 | 40f7035 | 2026-01-23 | 배포/설정 | [fix(config): enable overriding of environment variables when loading .env file](./07_stabilization_quality/198_40f7035.md) |
| 199 | 0b71f89 | 2026-01-29 | 시뮬레이션 | [fix(Step2EnvSetup): update expectedTotal only when API returns a valid value to prevent overwriting existing data](./07_stabilization_quality/199_0b71f89.md) |
| 200 | 54f1291 | 2026-01-29 | 보고서 에이전트 | [fix(report_agent): handle None responses from LLM during content generation and enforce fallback behavior](./07_stabilization_quality/200_54f1291.md) |
| 201 | f9abaf8 | 2026-02-06 | 보고서 에이전트 | [refactor(report_agent, Step4Report): simplify logging and remove subsection handling; update UI to reflect changes in section content generation](./07_stabilization_quality/201_f9abaf8.md) |
| 202 | e004fe8 | 2026-02-06 | 보고서 에이전트 | [fix(report_agent): update tool call requirements in content generation to allow up to 5 tool calls per chapter and clarify user prompts for insufficient data](./07_stabilization_quality/202_e004fe8.md) |
| 203 | 0a59bac | 2026-02-06 | 보고서 에이전트 | [fix(report_agent): increase minimum tool call requirement from 2 to 3 per chapter and enhance user prompts to encourage diverse tool usage](./07_stabilization_quality/203_0a59bac.md) |
| 204 | d2041f6 | 2026-02-14 | 보고서 에이전트 | [fix(report_agent): update description of insight_forge tool to remove "最强大" and enhance clarity](./07_stabilization_quality/204_d2041f6.md) |
| 205 | dc0a926 | 2026-02-14 | 보고서 에이전트 | [feat(report_agent): add detailed tool descriptions and prompts for future prediction report generation](./07_stabilization_quality/205_dc0a926.md) |
| 206 | 7601d78 | 2026-02-14 | 보고서 에이전트 | [feat(report_agent): enhance interview text processing and response handling; improve quote extraction and formatting for better clarity](./07_stabilization_quality/206_7601d78.md) |
| 207 | 709a0d7 | 2026-02-14 | 보고서 에이전트 | [feat(report_agent): enhance markdown rendering for lists and improve formatting; support nested lists and clean up HTML output](./07_stabilization_quality/207_709a0d7.md) |
| 208 | ddd9ff2 | 2026-02-14 | 보고서 에이전트 | [feat(report_agent): update report language consistency guidelines; ensure all quoted content is translated to the report language for clarity](./07_stabilization_quality/208_ddd9ff2.md) |
| 209 | ae1f38c | 2026-02-14 | 보고서 에이전트 | [fix(report_agent): improve markdown rendering by cleaning up <br> tags around block-level elements and enhancing list formatting](./07_stabilization_quality/209_ae1f38c.md) |
| 210 | 08ec856 | 2026-02-14 | 보고서 에이전트 | [fix(report_agent): update max_agents parameter description and enforce maximum limit of 10 agents](./07_stabilization_quality/210_08ec856.md) |
| 211 | 040c745 | 2026-02-22 | 문서/브랜딩 | [feat(readme): add Trendshift badge to README files for repository visibility](./07_stabilization_quality/211_040c745.md) |
| 212 | a795405 | 2026-02-22 | 문서/브랜딩 | [style(home): add overflow-y property to upload zone and adjust alignment for files](./07_stabilization_quality/212_a795405.md) |
| 213 | 25aa4f7 | 2026-02-24 | 보고서 에이전트 | [fix(report_agent): refine tool call handling and response validation; enforce strict separation between tool calls and final answers](./07_stabilization_quality/213_25aa4f7.md) |
| 214 | d30a0a2 | 2026-02-25 | 문서/브랜딩 | [Update README](./07_stabilization_quality/214_d30a0a2.md) |
| 215 | da6548e | 2026-02-27 | 그래프 | [feat(graph): implement pagination for fetching nodes and edges; add utility functions for streamlined data retrieval](./07_stabilization_quality/215_da6548e.md) |
| 216 | c6cea12 | 2026-02-27 | 시뮬레이션 | [docs(readme): add live demo section with link to online prediction simulation for both English and Chinese README files](./07_stabilization_quality/216_c6cea12.md) |
| 217 | 85b03d4 | 2026-02-27 | 문서/브랜딩 | [Update README](./07_stabilization_quality/217_85b03d4.md) |
| 218 | a1ff79c | 2026-03-05 | 문서/브랜딩 | [Update README](./07_stabilization_quality/218_a1ff79c.md) |
| 219 | 985f89f | 2026-03-06 | 백엔드 인프라 | [fix: resolve 500 error caused by <think> tags and markdown code fences in content field from reasoning models like MiniMax/GLM](./07_stabilization_quality/219_985f89f.md) |

