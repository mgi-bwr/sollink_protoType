# 로봇 통합 관제 서비스 UX/UI 디자인 원칙
_Exported on 2025. 10. 20. at 16시 5분 59초 GMT+9 from Cursor (1.6.45)_

---

**User**

@어드민 기본 구조.png 
이 이미지를 분석해서 로봇 통합 관제 서비스에 적용하기 위한 UX/UI 디자인 원칙을 json 형태로 정리해줘
이때 컨텐츠와 디자인 요소 (컬러, 텍스트, 레이아웃, 컴포넌트, 그외 모든것들) 을 연결지어서 맥락을 포함한 원칙으로 정리해줘

---

**Cursor**

이미지를 분석하여 디자인 원칙을 정리하겠습니다. 먼저 기존 프로젝트의 디자인 원칙 파일들을 참고하여 일관성 있는 형태로 작성하겠습니다.

이미지를 분석하여 로봇 통합 관제 서비스에 적용할 수 있는 포괄적인 UX/UI 디자인 원칙을 JSON 형태로 작성하겠습니다.

```json
{
  "솔링크_로봇통합관제_디자인원칙": {
    "문서정보": {
      "버전": "1.0",
      "작성일": "2025-10-20",
      "서비스명": "SOLink 로봇 통합 관제 서비스",
      "목적": "어드민 기본 구조 분석을 통한 로봇 관제 시스템 UI/UX 디자인 가이드라인",
      "적용대상": "관리자 인터페이스, 로봇 설정 관리, 데이터 관리, 사이트 관리"
    },

    "브랜드_아이덴티티": {
      "컬러_시스템": {
        "설명": "SOLink 브랜드 정체성과 관제 시스템의 기능적 요구사항을 반영한 색상 체계",
        
        "primary_brand": {
          "색상코드": "#00C896",
          "색상명": "SOLink Green",
          "적용영역": "브랜드 로고, 사이드바 로고 배경",
          "의미": "친환경 로봇 기술, 신뢰성, 혁신",
          "맥락": "사용자가 인터페이스에 접속하는 순간 SOLink 브랜드를 즉시 인식하도록 로고 영역에 집중 적용"
        },

        "primary_accent": {
          "색상코드": "#26C6DA",
          "색상명": "Cyan/Turquoise",
          "적용영역": "활성 메뉴 하이라이트, 주요 액션 버튼(로그아웃), CTA 버튼, 링크",
          "의미": "디지털 기술, 명확성, 현재 활성 상태",
          "맥락": "사용자의 현재 위치와 주요 액션을 명확하게 시각화하여 네비게이션 혼란 방지 및 중요 작업 강조"
        },

        "background_dark": {
          "색상코드": "#2B2D33",
          "색상명": "Dark Charcoal",
          "적용영역": "사이드바 배경, 네비게이션 영역",
          "의미": "전문성, 집중, 정보 계층 분리",
          "맥락": "관제 시스템의 전문적 이미지 구축 및 메인 컨텐츠와의 시각적 분리를 통한 정보 구조 명확화"
        },

        "background_light": {
          "색상코드": "#F5F7FA",
          "색상명": "Light Gray",
          "적용영역": "메인 컨텐츠 배경, 카드 배경",
          "의미": "깔끔함, 넓은 작업 공간, 가독성",
          "맥락": "장시간 관제 업무 시 눈의 피로도를 최소화하고 데이터 가독성을 극대화"
        },

        "content_white": {
          "색상코드": "#FFFFFF",
          "색상명": "Pure White",
          "적용영역": "입력 필드, 드롭다운, 카드, 모달",
          "의미": "입력 가능 영역, 상호작용 가능 요소",
          "맥락": "사용자가 조작할 수 있는 UI 요소를 명확히 구분하여 직관적인 인터랙션 유도"
        },

        "text_primary": {
          "dark_bg": "#FFFFFF",
          "light_bg": "#1A1C20",
          "의미": "주요 정보, 메뉴명, 페이지 타이틀",
          "맥락": "배경색에 따라 최적의 대비를 제공하여 WCAG 2.1 AA 기준 이상의 접근성 확보"
        },

        "text_secondary": {
          "dark_bg": "#A0A3A8",
          "light_bg": "#6C757D",
          "의미": "보조 정보, 메타데이터, 비활성 메뉴",
          "맥락": "정보의 우선순위를 시각적으로 계층화하여 사용자의 인지 부하 감소"
        },

        "semantic_colors": {
          "success": {
            "색상코드": "#28A745",
            "적용": "작업 완료, 로봇 정상 상태, 저장 성공",
            "맥락": "로봇 작업의 성공적 완료 및 시스템 정상 상태를 즉시 인식"
          },
          "warning": {
            "색상코드": "#FFC107",
            "적용": "주의 필요, 배터리 부족, 확인 요청",
            "맥락": "관제원의 주의가 필요한 상황을 경고 수준으로 알림"
          },
          "error": {
            "색상코드": "#DC3545",
            "적용": "로봇 오류, 작업 실패, 입력 오류",
            "맥락": "즉각적인 대응이 필요한 오류 상황을 강력하게 표시"
          },
          "info": {
            "색상코드": "#17A2B8",
            "적용": "정보성 알림, 시스템 안내, 도움말",
            "맥락": "사용자에게 유용한 정보를 제공하되 업무 흐름 방해 최소화"
          }
        }
      },

      "로고_시스템": {
        "primary_logo": {
          "구성": "녹색 배경(#00C896) + 'S' 아이콘 + SOLink 워드마크",
          "위치": "사이드바 최상단",
          "크기": "고정 높이 60-70px",
          "의미": "브랜드 인지도 강화 및 홈 버튼 역할",
          "맥락": "모든 관리 페이지에서 일관된 브랜드 경험 제공 및 빠른 홈 복귀 기능"
        }
      }
    },

    "레이아웃_구조": {
      "설명": "관제 시스템의 복잡한 정보를 효율적으로 조직화하는 레이아웃 원칙",

      "전체_구조": {
        "타입": "Fixed Sidebar + Fluid Content",
        "분할비율": "사이드바 200px 고정 / 메인 컨텐츠 가변",
        "의미": "안정적인 네비게이션과 유연한 작업 공간의 조화",
        "맥락": "다양한 화면 크기에서도 네비게이션의 일관성 유지하면서 컨텐츠 표시 최적화"
      },

      "사이드바_네비게이션": {
        "위치": "좌측 고정",
        "배경": "#2B2D33 (Dark Charcoal)",
        "너비": "200px",
        "스크롤": "독립 스크롤 가능",
        
        "구성요소": {
          "상단": {
            "요소": "SOLink 로고",
            "높이": "60-70px",
            "기능": "브랜드 표시 및 홈 링크",
            "맥락": "모든 페이지에서 브랜드 정체성 유지"
          },
          "중단": {
            "요소": "계층적 메뉴 구조",
            "구성": "아이콘 + 텍스트 레이블",
            "맥락": "관제 업무의 모든 기능 영역에 빠르게 접근"
          },
          "하단": {
            "요소": "로그아웃 버튼 + 버전 정보",
            "기능": "세션 관리 및 시스템 정보",
            "맥락": "보안 및 시스템 관리 기능의 접근성 확보"
          }
        },

        "메뉴_계층구조": {
          "1차_메뉴": {
            "구성": "아이콘(좌측) + 메뉴명 + 확장아이콘(우측, 하위 메뉴 있을 경우)",
            "아이콘_크기": "20x20px",
            "텍스트_크기": "14-15px",
            "패딩": "상하 12px, 좌우 16px",
            "호버_상태": "배경 밝아짐(#35373D)",
            "맥락": "명확한 시각적 피드백으로 클릭 가능 영역 표시"
          },
          "활성_메뉴": {
            "배경색": "#26C6DA (Cyan)",
            "텍스트색": "#FFFFFF",
            "아이콘색": "#FFFFFF",
            "의미": "현재 사용자가 위치한 페이지",
            "맥락": "사용자가 네비게이션 구조에서 자신의 위치를 명확히 인식"
          },
          "2차_메뉴": {
            "들여쓰기": "좌측 16px 추가",
            "배경": "투명",
            "텍스트_크기": "13-14px",
            "활성_표시": "좌측 강조선(#26C6DA, 3px)",
            "맥락": "계층 관계를 시각적으로 표현하여 정보 구조 이해 향상"
          }
        },

        "메뉴_항목_목록": {
          "설명": "로봇 관제 시스템의 기능별 분류",
          "항목": [
            "매뉴 관리 - 시스템 메뉴 설정 및 권한 연동",
            "권한 관리 - 사용자 역할 및 접근 권한 관리",
            "데이터 관리 - 로봇 및 관제 데이터 관리",
            "사이트 관리 - 운영 사이트 및 위치 정보 관리",
            "지도 관리 - 로봇 운행 지도 및 경로 관리",
            "회원 관리 - 시스템 사용자 및 권한 관리",
            "로봇 관리 - 로봇 등록, 설정, 모니터링",
            "POI 관리 - 관심 지점 및 작업 위치 관리",
            "알림 관리 - 알림 설정 및 수신자 관리",
            "AoD 관리 - AoD 디바이스 및 모델 관리",
            "문의 - 사용자 문의 및 지원",
            "도움말 - 시스템 가이드 및 매뉴얼"
          ],
          "맥락": "로봇 관제의 모든 관리 기능을 논리적으로 그룹화하여 학습 곡선 완화"
        }
      },

      "메인_컨텐츠_영역": {
        "위치": "사이드바 우측 전체",
        "배경": "#F5F7FA",
        "패딩": "24-32px",
        
        "상단_헤더": {
          "구성": "페이지 타이틀(좌측) + 사용자 아이콘(우측)",
          "높이": "60-80px",
          "페이지_타이틀": {
            "형식": "브레드크럼 (예: 알림 관리 / 수신자 주소록 관리)",
            "구분자": "/",
            "텍스트_크기": "20-24px",
            "폰트_굵기": "Bold",
            "의미": "현재 위치와 상위 컨텍스트 표시",
            "맥락": "복잡한 관리 구조에서 사용자의 위치 인식 및 컨텍스트 유지"
          },
          "사용자_정보": {
            "구성": "사용자 아이콘(원형)",
            "크기": "36-40px",
            "기능": "프로필 메뉴 트리거",
            "맥락": "빠른 계정 관리 및 설정 접근"
          }
        },

        "필터_섹션": {
          "위치": "컨텐츠 영역 최상단",
          "배경": "#FFFFFF 또는 #F8F9FA",
          "패딩": "16-20px",
          "테두리": "1px solid #E1E4E8",
          "구성": "드롭다운 + 검색 필드 + 버튼",
          "맥락": "대량의 로봇 및 관제 데이터에서 필요한 정보를 효율적으로 필터링"
        },

        "작업_영역": {
          "배경": "#FFFFFF",
          "패딩": "20-24px",
          "테두리반경": "4-8px",
          "그림자": "0 1px 3px rgba(0,0,0,0.1)",
          "의미": "주요 작업 및 데이터 표시 영역",
          "맥락": "시각적으로 구분된 작업 공간으로 사용자 집중도 향상"
        }
      },

      "반응형_전략": {
        "Desktop_1920px_이상": {
          "사이드바": "항상 표시 (200px 고정)",
          "컨텐츠": "최대 1720px 활용",
          "맥락": "관제실 대형 모니터 환경에서 최대 정보 밀도 제공"
        },
        "Laptop_1366px_1920px": {
          "사이드바": "항상 표시",
          "컨텐츠": "유연하게 조정",
          "맥락": "일반적인 관리자 노트북 환경 최적화"
        },
        "Tablet_768px_1365px": {
          "사이드바": "토글 가능 (햄버거 메뉴)",
          "컨텐츠": "전체 화면 활용",
          "맥락": "태블릿에서의 현장 관리 작업 지원"
        }
      }
    },

    "타이포그래피": {
      "설명": "정보의 명확한 전달과 시각적 계층을 위한 텍스트 시스템",

      "폰트_패밀리": {
        "primary": {
          "한글": "'Noto Sans KR', 'Malgun Gothic', sans-serif",
          "영문": "'Inter', 'Roboto', 'Helvetica Neue', sans-serif",
          "의미": "명확한 가독성과 전문적인 느낌",
          "맥락": "관제 데이터의 정확한 인식과 장시간 모니터링에서의 가독성 확보"
        },
        "monospace": {
          "사용": "'Roboto Mono', 'Courier New', monospace",
          "적용": "시간 데이터, 로봇 ID, 로그 정보",
          "맥락": "정렬이 필요한 숫자 및 코드 정보의 가독성 향상"
        }
      },

      "텍스트_스케일": {
        "heading_1": {
          "크기": "24px",
          "굵기": "700 (Bold)",
          "줄높이": "32px",
          "적용": "페이지 주 제목",
          "맥락": "사용자가 현재 작업 중인 주요 영역 명확히 인식"
        },
        "heading_2": {
          "크기": "20px",
          "굵기": "600 (SemiBold)",
          "줄높이": "28px",
          "적용": "섹션 제목, 카드 제목",
          "맥락": "컨텐츠 내 정보 영역 구분"
        },
        "heading_3": {
          "크기": "16px",
          "굵기": "600 (SemiBold)",
          "줄높이": "24px",
          "적용": "하위 섹션, 테이블 헤더",
          "맥락": "세부 정보 그룹 구분"
        },
        "body_large": {
          "크기": "15px",
          "굵기": "400 (Regular)",
          "줄높이": "24px",
          "적용": "주요 본문 텍스트, 데이터 표시",
          "맥락": "핵심 정보의 편안한 가독성"
        },
        "body_regular": {
          "크기": "14px",
          "굵기": "400 (Regular)",
          "줄높이": "22px",
          "적용": "일반 본문, 메뉴 텍스트",
          "맥락": "표준 정보 전달"
        },
        "body_small": {
          "크기": "13px",
          "굵기": "400 (Regular)",
          "줄높이": "20px",
          "적용": "보조 정보, 메타데이터",
          "맥락": "부가적 정보 표시"
        },
        "caption": {
          "크기": "12px",
          "굵기": "400 (Regular)",
          "줄높이": "18px",
          "적용": "라벨, 버전 정보, 타임스탬프",
          "맥락": "시스템 정보 및 미세한 안내"
        }
      },

      "텍스트_계층_원칙": {
        "primary_information": {
          "특징": "큰 크기, 진한 색상, 두꺼운 굵기",
          "예시": "로봇 이름, 작업 상태, 시간 정보",
          "맥락": "관제원이 즉시 인식해야 하는 핵심 데이터"
        },
        "secondary_information": {
          "특징": "중간 크기, 중간 색상, 보통 굵기",
          "예시": "로봇 모델명, 배터리 수준, 위치 정보",
          "맥락": "상황 파악을 위한 보조 정보"
        },
        "tertiary_information": {
          "특징": "작은 크기, 연한 색상, 가는 굵기",
          "예시": "마지막 업데이트 시간, 시스템 메시지",
          "맥락": "선택적으로 확인하는 메타데이터"
        }
      }
    },

    "컴포넌트_디자인": {
      "설명": "재사용 가능한 UI 요소들의 일관된 디자인 패턴",

      "버튼": {
        "primary_button": {
          "배경색": "#26C6DA",
          "텍스트색": "#FFFFFF",
          "높이": "36-40px",
          "패딩": "좌우 20-24px",
          "테두리반경": "4px",
          "호버": "배경색 10% 어둡게",
          "눌림": "배경색 15% 어둡게",
          "적용": "저장, 등록, 확인 등 주요 액션",
          "맥락": "사용자의 주요 작업 완료 유도 및 명확한 CTA 제공"
        },
        "secondary_button": {
          "배경색": "투명",
          "텍스트색": "#6C757D",
          "테두리": "1px solid #CED4DA",
          "높이": "36-40px",
          "패딩": "좌우 20-24px",
          "테두리반경": "4px",
          "호버": "배경색 #F8F9FA",
          "적용": "취소, 뒤로가기, 추가 옵션",
          "맥락": "보조 액션 제공하되 주요 액션과 시각적 우선순위 구분"
        },
        "danger_button": {
          "배경색": "#DC3545",
          "텍스트색": "#FFFFFF",
          "적용": "삭제, 제거, 초기화 등 파괴적 액션",
          "맥락": "위험한 작업임을 시각적으로 경고하여 실수 방지"
        },
        "text_button": {
          "배경색": "투명",
          "텍스트색": "#26C6DA",
          "테두리": "없음",
          "적용": "링크형 액션, 더보기, 접기/펼치기",
          "맥락": "경량 액션 제공 및 시각적 복잡도 최소화"
        },
        "icon_button": {
          "크기": "32x32px 또는 36x36px",
          "배경": "투명",
          "호버": "배경색 #F8F9FA",
          "적용": "편집, 삭제, 상세보기 등 테이블 내 액션",
          "맥락": "공간 효율적인 액션 버튼 배치"
        },
        "logout_button": {
          "배경색": "#26C6DA",
          "텍스트색": "#FFFFFF",
          "너비": "전체 (사이드바 내)",
          "높이": "44px",
          "위치": "사이드바 하단",
          "맥락": "중요한 보안 기능의 명확한 접근성 확보"
        }
      },

      "입력_필드": {
        "text_input": {
          "높이": "36-40px",
          "패딩": "좌우 12-16px",
          "배경색": "#FFFFFF",
          "테두리": "1px solid #CED4DA",
          "테두리반경": "4px",
          "포커스_테두리": "#26C6DA",
          "플레이스홀더_색상": "#ADB5BD",
          "맥락": "명확한 입력 영역 구분 및 포커스 상태 피드백"
        },
        "dropdown_select": {
          "구성": "선택값 + 드롭다운 화살표",
          "높이": "36-40px",
          "배경색": "#FFFFFF",
          "예시": "사이트 선택 드롭다운",
          "맥락": "제한된 옵션 중 선택하는 인터페이스 제공"
        },
        "search_field": {
          "구성": "검색 아이콘 + 입력 필드 + 검색 버튼",
          "플레이스홀더": "검색어를 입력하세요",
          "맥락": "대량 데이터에서 빠른 검색 기능 제공"
        },
        "validation_states": {
          "error": {
            "테두리": "#DC3545",
            "메시지색": "#DC3545",
            "아이콘": "경고 아이콘",
            "맥락": "입력 오류 즉시 피드백"
          },
          "success": {
            "테두리": "#28A745",
            "아이콘": "체크 아이콘",
            "맥락": "유효한 입력 확인"
          }
        }
      },

      "카드_컴포넌트": {
        "standard_card": {
          "배경색": "#FFFFFF",
          "패딩": "20-24px",
          "테두리반경": "8px",
          "그림자": "0 2px 4px rgba(0,0,0,0.08)",
          "테두리": "1px solid #E1E4E8",
          "맥락": "관련 정보를 그룹화하여 시각적 구조 제공"
        },
        "header": {
          "구성": "제목 + 액션 버튼",
          "하단_경계선": "1px solid #E1E4E8",
          "마진_하단": "16px",
          "맥락": "카드 내용의 컨텍스트 제공 및 빠른 액션 접근"
        }
      },

      "테이블": {
        "table_header": {
          "배경색": "#F8F9FA",
          "텍스트색": "#495057",
          "텍스트_굵기": "600 (SemiBold)",
          "높이": "48px",
          "패딩": "좌우 16px",
          "하단_경계선": "2px solid #DEE2E6",
          "맥락": "데이터 컬럼의 명확한 구분 및 정렬 기준 제공"
        },
        "table_row": {
          "높이": "52-56px",
          "패딩": "좌우 16px",
          "경계선": "1px solid #E9ECEF",
          "호버": "배경색 #F8F9FA",
          "맥락": "행 단위 데이터 그룹화 및 인터랙션 피드백"
        },
        "row_alternation": {
          "even_row": "#FFFFFF",
          "odd_row": "#FAFBFC",
          "적용": "선택적 (데이터 밀도 높을 때)",
          "맥락": "대량 데이터의 행 구분 가독성 향상"
        },
        "action_column": {
          "너비": "120-150px",
          "정렬": "중앙",
          "구성": "아이콘 버튼 조합",
          "맥락": "행별 작업 액션의 일관된 위치"
        }
      },

      "상태_배지": {
        "design": {
          "높이": "24px",
          "패딩": "좌우 10-12px",
          "테두리반경": "12px (pill shape)",
          "텍스트_크기": "12px",
          "텍스트_굵기": "500 (Medium)"
        },
        "types": {
          "success_badge": {
            "배경색": "#D4EDDA",
            "텍스트색": "#155724",
            "예시": "완료, 정상, 활성",
            "맥락": "긍정적 상태 즉시 인식"
          },
          "warning_badge": {
            "배경색": "#FFF3CD",
            "텍스트색": "#856404",
            "예시": "대기, 주의, 확인필요",
            "맥락": "주의 필요 상태 표시"
          },
          "error_badge": {
            "배경색": "#F8D7DA",
            "텍스트색": "#721C24",
            "예시": "오류, 실패, 중단",
            "맥락": "문제 상태 강조"
          },
          "info_badge": {
            "배경색": "#D1ECF1",
            "텍스트색": "#0C5460",
            "예시": "진행중, 예약",
            "맥락": "중립적 상태 정보"
          }
        }
      },

      "모달_다이얼로그": {
        "overlay": {
          "배경색": "rgba(0, 0, 0, 0.5)",
          "의미": "현재 작업에 집중 유도",
          "맥락": "중요한 작업 또는 확인이 필요한 상황"
        },
        "modal_container": {
          "배경색": "#FFFFFF",
          "최대_너비": "600px",
          "테두리반경": "8px",
          "그림자": "0 10px 40px rgba(0,0,0,0.15)",
          "패딩": "24-32px"
        },
        "modal_header": {
          "제목_크기": "20px",
          "제목_굵기": "600 (SemiBold)",
          "닫기_버튼": "우측 상단 X 아이콘"
        },
        "modal_footer": {
          "정렬": "우측",
          "버튼_간격": "8-12px",
          "구성": "취소 + 확인 버튼",
          "맥락": "명확한 의사결정 유도"
        }
      },

      "탭_네비게이션": {
        "tab_container": {
          "하단_경계선": "1px solid #DEE2E6",
          "맥락": "관련 컨텐츠를 그룹화하여 공간 효율적 구성"
        },
        "tab_item": {
          "패딩": "상하 12px, 좌우 20px",
          "텍스트_크기": "14px",
          "비활성_색상": "#6C757D",
          "활성_색상": "#26C6DA",
          "활성_하단선": "3px solid #26C6DA",
          "맥락": "현재 보고 있는 정보 범위 명확화"
        }
      },

      "아이콘_시스템": {
        "스타일": "Line icons (Outlined)",
        "크기": {
          "small": "16x16px",
          "medium": "20x20px",
          "large": "24x24px"
        },
        "색상": "현재 텍스트 색상 상속",
        "적용": "메뉴, 버튼, 상태 표시",
        "맥락": "시각적 인식 속도 향상 및 언어 장벽 완화"
      }
    },

    "인터랙션_패턴": {
      "설명": "사용자와 시스템 간 상호작용의 일관된 행동 규칙",

      "네비게이션_인터랙션": {
        "메뉴_클릭": {
          "동작": "즉시 페이지 전환",
          "피드백": "활성 메뉴 하이라이트 업데이트",
          "맥락": "빠른 화면 전환으로 관제 효율성 향상"
        },
        "하위_메뉴_확장": {
          "트리거": "펼치기 아이콘 또는 부모 메뉴 클릭",
          "애니메이션": "0.2s 부드러운 펼침",
          "상태_유지": "페이지 이동 후에도 확장 상태 유지",
          "맥락": "복잡한 메뉴 구조의 직관적 탐색"
        },
        "로고_클릭": {
          "동작": "홈 또는 대시보드로 이동",
          "맥락": "빠른 초기 화면 복귀"
        }
      },

      "데이터_조작": {
        "필터_적용": {
          "트리거": "검색 버튼 클릭 또는 Enter 키",
          "로딩_표시": "스피너 또는 스켈레톤 UI",
          "결과_표시": "즉시 테이블 업데이트",
          "맥락": "대량 데이터에서 원하는 정보 빠른 추출"
        },
        "정렬": {
          "트리거": "테이블 헤더 클릭",
          "표시": "정렬 방향 아이콘 (↑↓)",
          "맥락": "데이터 분석 및 비교 용이"
        },
        "페이지네이션": {
          "위치": "테이블 하단 중앙 또는 우측",
          "구성": "이전/다음 버튼 + 페이지 번호",
          "맥락": "대량 데이터의 효율적 탐색"
        }
      },

      "폼_인터랙션": {
        "실시간_검증": {
          "시점": "입력 필드 포커스 아웃 시",
          "피드백": "에러 메시지 + 색상 변경",
          "맥락": "입력 오류 조기 발견 및 수정"
        },
        "저장_프로세스": {
          "단계": "저장 버튼 클릭 → 로딩 표시 → 성공/실패 토스트",
          "버튼_상태": "로딩 중 비활성화",
          "맥락": "중복 제출 방지 및 명확한 피드백"
        },
        "취소_동작": {
          "확인": "변경사항 있을 경우 확인 다이얼로그",
          "맥락": "실수로 인한 데이터 손실 방지"
        }
      },

      "호버_및_포커스": {
        "원칙": "모든 클릭 가능 요소에 호버/포커스 상태 제공",
        "시각적_피드백": {
          "버튼": "배경색 변경 + 커서 pointer",
          "링크": "언더라인 + 색상 변경",
          "테이블_행": "배경색 밝아짐",
          "입력_필드": "테두리 색상 변경 + 그림자"
        },
        "맥락": "인터랙티브 요소 명확히 구분하여 사용성 향상"
      },

      "로딩_상태": {
        "전체_페이지_로딩": {
          "표시": "중앙 스피너 + 반투명 오버레이",
          "맥락": "초기 데이터 로드 중"
        },
        "부분_로딩": {
          "표시": "스켈레톤 UI 또는 영역별 스피너",
          "맥락": "특정 컴포넌트 데이터 갱신 중"
        },
        "버튼_로딩": {
          "표시": "버튼 내 작은 스피너 + 텍스트 변경",
          "맥락": "비동기 작업 진행 중"
        }
      },

      "피드백_시스템": {
        "토스트_알림": {
          "위치": "화면 우측 상단 또는 중앙 상단",
          "지속시간": "3-5초 (자동 사라짐)",
          "타입": "성공/경고/오류/정보",
          "맥락": "작업 결과의 즉각적 피드백"
        },
        "인라인_메시지": {
          "위치": "해당 입력 필드 하단",
          "타입": "에러 또는 안내 메시지",
          "맥락": "컨텍스트 내 즉각적 피드백"
        },
        "확인_다이얼로그": {
          "용도": "삭제, 초기화 등 중요 작업",
          "구성": "제목 + 설명 + 취소/확인 버튼",
          "맥락": "실수 방지 및 의도 재확인"
        }
      },

      "드래그_앤_드롭": {
        "적용": "순서 변경, 파일 업로드",
        "시각적_피드백": "드래그 중 반투명 + 드롭 가능 영역 하이라이트",
        "맥락": "직관적인 조작으로 사용성 향상"
      }
    },

    "정보_아키텍처": {
      "설명": "복잡한 로봇 관제 정보를 논리적으로 조직화하는 원칙",

      "계층적_구조": {
        "레벨_1": {
          "내용": "주요 관리 영역 (메뉴 관리, 데이터 관리, 로봇 관리 등)",
          "표현": "사이드바 1차 메뉴",
          "맥락": "관제 업무의 큰 범주 구분"
        },
        "레벨_2": {
          "내용": "세부 기능 (알림 설정, 주소록 관리 등)",
          "표현": "사이드바 2차 메뉴 또는 페이지 내 탭",
          "맥락": "특정 관리 작업 선택"
        },
        "레벨_3": {
          "내용": "구체적 작업 (수신자 등록, 알림 활성화 등)",
          "표현": "페이지 내 폼 또는 모달",
          "맥락": "실제 데이터 조작"
        }
      },

      "브레드크럼_네비게이션": {
        "형식": "상위카테고리 / 현재페이지",
        "예시": "알림 관리 / 수신자 주소록 관리",
        "구분자": "/",
        "링크": "상위 카테고리는 클릭 가능",
        "맥락": "복잡한 구조에서 사용자의 위치 인식 및 상위 레벨로 빠른 이동"
      },

      "정보_그룹화": {
        "원칙": "관련 정보를 카드 또는 섹션으로 그룹화",
        "시각적_구분": "배경색, 경계선, 여백",
        "맥락": "정보 덩어리(chunk)를 만들어 인지 부하 감소"
      },

      "검색_가능성": {
        "글로벌_검색": "헤더 영역의 전체 검색",
        "로컬_검색": "페이지 내 데이터 필터링",
        "맥락": "대량의 로봇 및 사이트 정보에서 빠른 접근"
      }
    },

    "접근성_및_사용성": {
      "설명": "모든 사용자가 효율적으로 시스템을 사용할 수 있도록 하는 원칙",

      "색상_대비": {
        "원칙": "WCAG 2.1 AA 기준 이상 준수",
        "일반_텍스트": "4.5:1 이상",
        "큰_텍스트": "3:1 이상",
        "맥락": "다양한 시력 조건에서도 정보 인식 가능"
      },

      "키보드_네비게이션": {
        "Tab_순서": "논리적 흐름 (좌상단 → 우하단)",
        "포커스_표시": "명확한 아웃라인 (2px solid #26C6DA)",
        "단축키": "주요 기능에 대한 키보드 단축키 제공",
        "맥락": "마우스 없이도 모든 기능 접근 가능"
      },

      "스크린_리더": {
        "ARIA_라벨": "의미있는 요소에 적절한 라벨 제공",
        "랜드마크": "주요 영역에 role 속성 적용",
        "동적_콘텐츠": "변경 사항 알림 (aria-live)",
        "맥락": "시각 장애인도 시스템 사용 가능"
      },

      "에러_처리": {
        "명확한_메시지": "문제점과 해결 방법 설명",
        "위치_표시": "에러 발생 필드 명확히 표시",
        "복구_옵션": "사용자가 쉽게 수정할 수 있도록 안내",
        "맥락": "사용자 좌절 최소화 및 빠른 문제 해결"
      },

      "반응_시간": {
        "즉각적_피드백": "100ms 이내",
        "간단한_작업": "1초 이내",
        "복잡한_작업": "10초 이내 (진행 표시 포함)",
        "맥락": "시스템 반응성에 대한 사용자 만족도 유지"
      },

      "학습_곡선": {
        "일관성": "유사 기능은 유사한 UI 패턴 사용",
        "예측_가능성": "표준 UI 컨벤션 준수",
        "도움말": "컨텍스트 기반 도움말 및 툴팁 제공",
        "맥락": "신규 관리자의 빠른 시스템 적응"
      }
    },

    "성능_최적화": {
      "설명": "빠르고 반응성 좋은 사용자 경험을 위한 원칙",

      "데이터_로딩": {
        "지연_로딩": "화면에 보이는 데이터만 우선 로드",
        "무한_스크롤": "페이지네이션 대신 무한 스크롤 적용 (선택적)",
        "캐싱": "자주 사용되는 데이터 클라이언트 캐싱",
        "맥락": "대량의 로봇 데이터 효율적 처리"
      },

      "검색_최적화": {
        "디바운싱": "검색 입력 후 300ms 대기",
        "자동완성": "입력 중 실시간 제안",
        "맥락": "불필요한 API 호출 감소"
      },

      "이미지_최적화": {
        "지연_로딩": "뷰포트 진입 시 로드",
        "적절한_포맷": "WebP 우선, PNG/JPG 폴백",
        "반응형_이미지": "화면 크기에 맞는 이미지 제공",
        "맥락": "페이지 로드 속도 향상"
      }
    },

    "콘텐츠_전략": {
      "설명": "효과적인 정보 전달을 위한 콘텐츠 원칙",

      "용어_일관성": {
        "원칙": "시스템 전반에서 동일한 용어 사용",
        "예시": {
          "로봇": "Robot (일관되게 사용)",
          "사이트": "Site (건물/지역)",
          "작업": "Task/Job",
          "관제": "Control/Monitoring"
        },
        "맥락": "관리자 간 명확한 의사소통 및 학습 효율"
      },

      "메시지_톤": {
        "전문적": "B2B 관제 시스템에 적합한 전문적 어조",
        "명확함": "모호하지 않은 직접적 표현",
        "긍정적": "사용자 행동 유도 시 긍정적 언어",
        "맥락": "신뢰성 있는 시스템 이미지 구축"
      },

      "에러_메시지": {
        "구조": "문제 설명 + 원인 + 해결 방법",
        "예시": "로봇을 찾을 수 없습니다. 로봇 ID를 확인하거나 관리자에게 문의하세요.",
        "맥락": "사용자가 스스로 문제 해결 가능"
      },

      "빈_상태": {
        "표시": "데이터 없음 메시지 + 액션 버튼",
        "예시": "등록된 로봇이 없습니다. [로봇 추가] 버튼을 클릭하세요.",
        "맥락": "사용자에게 다음 행동 제안"
      }
    },

    "확장성_및_유지보수": {
      "설명": "장기적인 시스템 발전을 위한 설계 원칙",

      "컴포넌트_재사용": {
        "원칙": "동일 기능은 동일 컴포넌트 재사용",
        "라이브러리": "공통 UI 컴포넌트 라이브러리 구축",
        "맥락": "개발 효율성 및 일관성 유지"
      },

      "테마_시스템": {
        "색상_변수": "CSS Custom Properties 또는 디자인 토큰 사용",
        "다크_모드": "다크 모드 지원 고려 (선택적)",
        "맥락": "브랜드 변경 또는 사용자 선호도 대응"
      },

      "문서화": {
        "디자인_시스템": "모든 컴포넌트의 사용법 문서화",
        "코드_주석": "복잡한 로직에 명확한 주석",
        "맥락": "팀 협업 및 유지보수 효율성"
      },

      "버전_관리": {
        "표시": "사이드바 하단에 버전 정보 표시",
        "예시": "Version 3.0",
        "맥락": "시스템 버전 추적 및 지원"
      }
    },

    "모바일_태블릿_고려사항": {
      "설명": "다양한 디바이스 환경 지원",

      "터치_인터랙션": {
        "터치_영역": "최소 44x44px",
        "제스처": "스와이프, 핀치 줌 지원 (지도 등)",
        "맥락": "현장에서 태블릿으로 관리 작업 수행"
      },

      "사이드바_적응": {
        "모바일": "햄버거 메뉴로 전환, 오버레이 표시",
        "태블릿": "토글 가능, 아이콘만 표시 옵션",
        "맥락": "작은 화면에서 컨텐츠 공간 최대화"
      }
    },

    "보안_및_권한": {
      "설명": "안전한 관제 시스템 운영을 위한 UI 원칙",

      "권한_기반_UI": {
        "원칙": "권한 없는 기능은 숨김 또는 비활성화",
        "표시": "권한 부족 시 명확한 안내 메시지",
        "맥락": "불필요한 기능 노출 방지 및 명확한 권한 구조"
      },

      "세션_관리": {
        "로그아웃": "명확한 로그아웃 버튼 (사이드바 하단)",
        "세션_만료": "만료 전 경고 + 연장 옵션",
        "맥락": "보안 유지 및 작업 손실 방지"
      },

      "민감_정보_표시": {
        "마스킹": "필요시 정보 일부 마스킹",
        "권한_확인": "중요 작업 전 비밀번호 재확인",
        "맥락": "데이터 보안 강화"
      }
    },

    "특정_시나리오_적용": {
      "설명": "로봇 관제 특화 시나리오별 디자인 가이드",

      "사이트_선택_시나리오": {
        "UI": "드롭다운 선택 컴포넌트",
        "위치": "컨텐츠 영역 최상단",
        "동작": "선택 시 해당 사이트 데이터로 즉시 필터링",
        "맥락": "다중 사이트 관리 시 컨텍스트 명확화"
      },

      "로봇_상태_모니터링": {
        "실시간_업데이트": "WebSocket 기반 실시간 데이터 반영",
        "상태_색상": "정상(녹색), 경고(노랑), 오류(빨강)",
        "알림": "중요 상태 변경 시 토스트 알림",
        "맥락": "로봇 이상 상황 즉시 감지 및 대응"
      },

      "작업_이력_조회": {
        "필터": "날짜 범위, 로봇, 작업 유형",
        "정렬": "시간순 기본 정렬, 클릭으로 변경 가능",
        "상세보기": "행 클릭 또는 확장 버튼",
        "맥락": "과거 작업 분석 및 문제 추적"
      },

      "알림_관리": {
        "수신자_선택": "다중 선택 체크박스",
        "로봇_연결": "드래그 앤 드롭 또는 선택 UI",
        "활성화_토글": "스위치 컴포넌트",
        "맥락": "유연한 알림 설정 및 관리"
      }
    },

    "디자인_검증_체크리스트": {
      "설명": "디자인 구현 시 확인해야 할 핵심 항목",

      "일관성_확인": [
        "모든 페이지에서 동일한 헤더/사이드바 구조 사용",
        "버튼 스타일이 전체 시스템에서 일관됨",
        "색상 사용이 디자인 시스템 규칙을 따름",
        "타이포그래피 스케일이 일관되게 적용됨"
      ],

      "기능성_확인": [
        "모든 인터랙티브 요소가 호버/포커스 상태를 가짐",
        "로딩 상태가 명확히 표시됨",
        "에러 상황에서 적절한 피드백 제공",
        "폼 검증이 실시간으로 작동함"
      ],

      "접근성_확인": [
        "키보드만으로 모든 기능 사용 가능",
        "색상 대비가 WCAG 기준 충족",
        "모든 이미지와 아이콘에 alt 텍스트 제공",
        "ARIA 속성이 적절히 사용됨"
      ],

      "성능_확인": [
        "초기 페이지 로드 시간 3초 이내",
        "인터랙션 반응 시간 100ms 이내",
        "대량 데이터 테이블이 부드럽게 스크롤됨",
        "이미지가 최적화되어 있음"
      ]
    }
  }
}

```

완료했습니다! 

제공하신 "어드민 기본 구조.png" 이미지를 분석하여 **로봇 통합 관제 서비스에 적용하기 위한 포괄적인 UX/UI 디자인 원칙**을 JSON 형태로 작성했습니다.

## 📋 작성된 파일
`/Users/mgi/Documents/개발팀/솔링크/3.0~/prd2wirefram/admin_cleaningRobot_exapandablesSetting/robot_control_design_principles.json`

## 🎨 주요 내용

### 1. **브랜드 아이덴티티**
- **컬러 시스템**: SOLink Green (#00C896), Cyan (#26C6DA), 다크/라이트 배경색, 시맨틱 컬러 등
- 각 색상의 적용 영역, 의미, 맥락을 상세히 정리

### 2. **레이아웃 구조**
- 좌측 고정 사이드바 (200px) + 유동적 메인 컨텐츠 영역
- 사이드바 메뉴 계층 구조 (1차/2차 메뉴, 활성 상태)
- 반응형 전략 (Desktop, Laptop, Tablet)

### 3. **타이포그래피**
- 폰트 패밀리, 텍스트 스케일 (Heading 1-3, Body Large/Regular/Small, Caption)
- 텍스트 계층 원칙 (Primary/Secondary/Tertiary Information)

### 4. **컴포넌트 디자인**
- 버튼 (Primary, Secondary, Danger, Text, Icon, Logout)
- 입력 필드 (Text Input, Dropdown, Search, Validation)
- 카드, 테이블, 상태 배지, 모달, 탭, 아이콘 시스템

### 5. **인터랙션 패턴**
- 네비게이션, 데이터 조작, 폼 인터랙션
- 호버/포커스 상태, 로딩 상태, 피드백 시스템

### 6. **정보 아키텍처**
- 계층적 구조 (3레벨), 브레드크럼 네비게이션
- 정보 그룹화, 검색 가능성

### 7. **접근성 & 사용성**
- WCAG 2.1 AA 기준 준수, 키보드 네비게이션
- 스크린 리더 지원, 에러 처리

### 8. **특정 시나리오 적용**
- 사이트 선택, 로봇 상태 모니터링
- 작업 이력 조회, 알림 관리

## ✨ 특징

모든 디자인 요소에 **"맥락(context)"**을 포함하여:
- 왜 이 색상을 사용하는지
- 왜 이 레이아웃 구조를 선택했는지
- 사용자 경험에 어떤 영향을 미치는지

를 명확히 설명했습니다. 이를 통해 개발팀이 단순히 디자인을 따라하는 것이 아니라, **디자인 결정의 이유를 이해**하고 일관성 있게 적용할 수 있도록 했습니다.

---

**User**

@robot_control_design_principles.json @어드민 기본 구조.png @PRD.txt 
PRD와 앞서 작성한 디자인 원칙을 토대로, 소모품 관리 기능 샘플 페이지를 개발해줘

- 이때 샘플 페이지는 PRD에서 규정한 기능이 어떻게 작동되는지 확인할 수 있는 프로토타입이어야해
- 또한, 어드민 기본 구조 이미지에서 제공한것과 기본 레이아웃은 동일하되 '콘텐츠 영역 (개발 필요)'라고 명시된 영역에 실제 소모품 관리에 대한 내용이 적용되어야해
- UI와 전반적인 페이지의 레이아웃은 Tailwind CSS를 기반으로 구현해줘
- PRD에 명시되어 있지 않은 사항은 구현 범위에서 제외되어야 해


---

**Cursor**

PRD와 디자인 원칙을 기반으로 소모품 관리 기능 샘플 페이지를 개발하겠습니다.

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>소모품 관리 - SOLink 로봇 통합 관제</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
        }
        
        /* 사이드바 스크롤 */
        .sidebar-scroll {
            overflow-y: auto;
            scrollbar-width: thin;
            scrollbar-color: #4A4D55 #2B2D33;
        }
        
        .sidebar-scroll::-webkit-scrollbar {
            width: 6px;
        }
        
        .sidebar-scroll::-webkit-scrollbar-track {
            background: #2B2D33;
        }
        
        .sidebar-scroll::-webkit-scrollbar-thumb {
            background: #4A4D55;
            border-radius: 3px;
        }

        /* 메뉴 호버 효과 */
        .menu-item:hover {
            background-color: #35373D;
        }

        /* 상태 배지 애니메이션 */
        .status-badge {
            transition: all 0.2s ease;
        }

        /* 토스트 애니메이션 */
        @keyframes slideIn {
            from {
                transform: translateX(100%);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .toast {
            animation: slideIn 0.3s ease-out;
        }

        /* 모달 애니메이션 */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        .modal-overlay {
            animation: fadeIn 0.2s ease-out;
        }

        /* 테이블 행 호버 */
        .table-row:hover {
            background-color: #F8F9FA;
        }

        /* 검색 아이콘 */
        .search-icon {
            pointer-events: none;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- 레이아웃 컨테이너 -->
    <div class="flex min-h-screen">
        <!-- 사이드바 -->
        <aside class="w-[200px] bg-[#2B2D33] text-white flex flex-col fixed h-screen">
            <!-- 로고 -->
            <div class="h-[70px] bg-[#00C896] flex items-center justify-center cursor-pointer">
                <div class="flex items-center space-x-2">
                    <div class="w-8 h-8 bg-white rounded flex items-center justify-center">
                        <span class="text-[#00C896] font-bold text-xl">S</span>
                    </div>
                    <span class="text-white font-bold text-lg">SOLink</span>
                </div>
            </div>

            <!-- 메뉴 영역 -->
            <nav class="flex-1 sidebar-scroll py-4">
                <div class="px-3 space-y-1">
                    <!-- 메뉴 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>📋</span>
                            <span>매뉴 관리</span>
                        </div>
                    </div>

                    <!-- 권한 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>🔐</span>
                            <span>권한 관리</span>
                        </div>
                    </div>

                    <!-- 데이터 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>📊</span>
                            <span>데이터 관리</span>
                        </div>
                    </div>

                    <!-- 사이트 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>🏢</span>
                            <span>사이트 관리</span>
                        </div>
                    </div>

                    <!-- 지도 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>🗺️</span>
                            <span>지도 관리</span>
                        </div>
                    </div>

                    <!-- 회원 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>👥</span>
                            <span>회원 관리</span>
                        </div>
                    </div>

                    <!-- 로봇 관리 - 활성 -->
                    <div class="bg-[#26C6DA] px-4 py-3 rounded cursor-pointer text-sm">
                        <div class="flex items-center space-x-3">
                            <span>🤖</span>
                            <span>로봇 관리</span>
                        </div>
                    </div>

                    <!-- POI 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>📍</span>
                            <span>POI 관리</span>
                        </div>
                    </div>

                    <!-- 알림 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>🔔</span>
                            <span>알림 관리</span>
                        </div>
                    </div>

                    <!-- AoD 관리 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>📱</span>
                            <span>AoD 관리</span>
                        </div>
                    </div>

                    <!-- 문의 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>❓</span>
                            <span>문의</span>
                        </div>
                    </div>

                    <!-- 도움말 -->
                    <div class="menu-item px-4 py-3 rounded cursor-pointer flex items-center justify-between text-sm text-[#A0A3A8]">
                        <div class="flex items-center space-x-3">
                            <span>📖</span>
                            <span>도움말</span>
                        </div>
                    </div>
                </div>
            </nav>

            <!-- 로그아웃 버튼 & 버전 정보 -->
            <div class="p-4 space-y-2">
                <button class="w-full bg-[#26C6DA] hover:bg-[#21B1C4] text-white py-3 rounded font-medium transition-colors">
                    로그아웃
                </button>
                <div class="text-center text-xs text-[#6C757D]">
                    Version 3.0<br>
                    © Bigwave Robotics Inc. All Rights Reserved.
                </div>
            </div>
        </aside>

        <!-- 메인 컨텐츠 -->
        <main class="ml-[200px] flex-1 bg-[#F5F7FA]">
            <!-- 상단 헤더 -->
            <header class="bg-white border-b border-gray-200 h-[70px] flex items-center justify-between px-8">
                <h1 class="text-2xl font-bold text-[#1A1C20]">로봇 관리 / 소모품 관리</h1>
                <div class="w-10 h-10 bg-gray-300 rounded-full flex items-center justify-center cursor-pointer">
                    <span class="text-gray-600">👤</span>
                </div>
            </header>

            <!-- 컨텐츠 영역 -->
            <div class="p-8">
                <!-- 필터 섹션 -->
                <div class="bg-white rounded-lg border border-[#E1E4E8] p-5 mb-6">
                    <div class="flex items-center space-x-4">
                        <label class="text-sm font-semibold text-[#495057] min-w-[80px]">사이트 선택</label>
                        <div class="flex-1 max-w-xs">
                            <select id="siteSelect" class="w-full h-10 px-4 border border-[#CED4DA] rounded focus:outline-none focus:border-[#26C6DA] text-sm">
                                <option value="all">사이트 전체</option>
                                <option value="site-a">사이트 A</option>
                                <option value="site-b">사이트 B</option>
                                <option value="site-c">사이트 C</option>
                                <option value="site-d">서울 본사</option>
                                <option value="site-e">부산 지사</option>
                            </select>
                        </div>
                    </div>
                </div>

                <!-- 청소로봇 목록 카드 -->
                <div class="bg-white rounded-lg border border-[#E1E4E8] shadow-sm">
                    <!-- 카드 헤더 -->
                    <div class="border-b border-[#E1E4E8] p-5">
                        <div class="flex items-center justify-between">
                            <h2 class="text-lg font-semibold text-[#1A1C20]">청소로봇 목록</h2>
                            <div class="relative">
                                <input 
                                    type="text" 
                                    id="robotSearch" 
                                    placeholder="로봇명 검색..." 
                                    class="w-64 h-10 pl-10 pr-4 border border-[#CED4DA] rounded focus:outline-none focus:border-[#26C6DA] text-sm"
                                >
                                <svg class="absolute left-3 top-1/2 transform -translate-y-1/2 w-4 h-4 text-gray-400 search-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                                </svg>
                            </div>
                        </div>
                    </div>

                    <!-- 테이블 -->
                    <div class="overflow-x-auto">
                        <table class="w-full">
                            <thead class="bg-[#F8F9FA]">
                                <tr>
                                    <th class="px-6 py-4 text-left text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">No.</th>
                                    <th class="px-6 py-4 text-left text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">사이트명</th>
                                    <th class="px-6 py-4 text-left text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">로봇 모델명</th>
                                    <th class="px-6 py-4 text-left text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">로봇명</th>
                                    <th class="px-6 py-4 text-left text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">소모품 종합 상태</th>
                                    <th class="px-6 py-4 text-center text-sm font-semibold text-[#495057] border-b-2 border-[#DEE2E6]">관리</th>
                                </tr>
                            </thead>
                            <tbody id="robotTableBody">
                                <!-- Row 1 -->
                                <tr class="table-row border-b border-[#E9ECEF]">
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">5</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">사이트 A</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">Clean-X Pro</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">청소로봇-A01</td>
                                    <td class="px-6 py-4">
                                        <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-medium bg-[#F8D7DA] text-[#721C24]">
                                            교체 필요
                                        </span>
                                    </td>
                                    <td class="px-6 py-4 text-center">
                                        <button onclick="openDetailModal('청소로봇-A01', 'Clean-X Pro', 'replace')" class="text-[#26C6DA] hover:text-[#21B1C4] font-medium text-sm">
                                            상세 관리
                                        </button>
                                    </td>
                                </tr>
                                <!-- Row 2 -->
                                <tr class="table-row border-b border-[#E9ECEF]">
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">4</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">사이트 A</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">Clean-X Pro</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">청소로봇-A02</td>
                                    <td class="px-6 py-4">
                                        <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-medium bg-[#FFF3CD] text-[#856404]">
                                            주의
                                        </span>
                                    </td>
                                    <td class="px-6 py-4 text-center">
                                        <button onclick="openDetailModal('청소로봇-A02', 'Clean-X Pro', 'warning')" class="text-[#26C6DA] hover:text-[#21B1C4] font-medium text-sm">
                                            상세 관리
                                        </button>
                                    </td>
                                </tr>
                                <!-- Row 3 -->
                                <tr class="table-row border-b border-[#E9ECEF]">
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">3</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">사이트 B</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">Clean-Y</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">청소로봇-B01</td>
                                    <td class="px-6 py-4">
                                        <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-medium bg-[#D4EDDA] text-[#155724]">
                                            정상
                                        </span>
                                    </td>
                                    <td class="px-6 py-4 text-center">
                                        <button onclick="openDetailModal('청소로봇-B01', 'Clean-Y', 'normal')" class="text-[#26C6DA] hover:text-[#21B1C4] font-medium text-sm">
                                            상세 관리
                                        </button>
                                    </td>
                                </tr>
                                <!-- Row 4 -->
                                <tr class="table-row border-b border-[#E9ECEF]">
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">2</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">사이트 C</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">Clean-Z Mini</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">청소로봇-C01</td>
                                    <td class="px-6 py-4">
                                        <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-medium bg-[#D1ECF1] text-[#0C5460]">
                                            사용중인 소모품 없음
                                        </span>
                                    </td>
                                    <td class="px-6 py-4 text-center">
                                        <button onclick="openDetailModal('청소로봇-C01', 'Clean-Z Mini', 'none')" class="text-[#26C6DA] hover:text-[#21B1C4] font-medium text-sm">
                                            상세 관리
                                        </button>
                                    </td>
                                </tr>
                                <!-- Row 5 -->
                                <tr class="table-row">
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">1</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">사이트 C</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">Clean-Z Mini</td>
                                    <td class="px-6 py-4 text-sm text-[#1A1C20]">청소로봇-C02</td>
                                    <td class="px-6 py-4">
                                        <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-medium bg-[#D4EDDA] text-[#155724]">
                                            정상
                                        </span>
                                    </td>
                                    <td class="px-6 py-4 text-center">
                                        <button onclick="openDetailModal('청소로봇-C02', 'Clean-Z Mini', 'normal')" class="text-[#26C6DA] hover:text-[#21B1C4] font-medium text-sm">
                                            상세 관리
                                        </button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </main>
    </div>

    <!-- 소모품 상세 관리 모달 -->
    <div id="detailModal" class="fixed inset-0 bg-black bg-opacity-50 hidden items-center justify-center z-50 modal-overlay">
        <div class="bg-white rounded-lg shadow-xl max-w-4xl w-full mx-4 max-h-[90vh] overflow-y-auto">
            <!-- 모달 헤더 -->
            <div class="border-b border-[#E1E4E8] p-6 flex items-center justify-between sticky top-0 bg-white">
                <div>
                    <h3 class="text-xl font-semibold text-[#1A1C20]" id="modalTitle">청소로봇 소모품 상세 관리</h3>
                    <p class="text-sm text-[#6C757D] mt-1" id="modalSubtitle">로봇명: 청소로봇-A01 (모델: Clean-X Pro)</p>
                </div>
                <button onclick="closeDetailModal()" class="text-gray-400 hover:text-gray-600">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                    </svg>
                </button>
            </div>

            <!-- 모달 본문 -->
            <div class="p-6 space-y-6" id="consumablesForm">
                <!-- 소모품 항목들이 여기에 동적으로 추가됩니다 -->
            </div>

            <!-- 모달 푸터 -->
            <div class="border-t border-[#E1E4E8] p-6 flex justify-end space-x-3 sticky bottom-0 bg-white">
                <button onclick="closeDetailModal()" class="px-6 py-2 border border-[#CED4DA] rounded text-[#6C757D] hover:bg-[#F8F9FA] font-medium">
                    취소
                </button>
                <button onclick="saveConsumables()" class="px-6 py-2 bg-[#26C6DA] hover:bg-[#21B1C4] text-white rounded font-medium">
                    저장하기
                </button>
            </div>
        </div>
    </div>

    <!-- 토스트 알림 -->
    <div id="toast" class="fixed top-8 right-8 bg-white border border-[#E1E4E8] rounded-lg shadow-lg p-4 hidden toast z-50 min-w-[300px]">
        <div class="flex items-start">
            <div id="toastIcon" class="mr-3"></div>
            <div class="flex-1">
                <p id="toastMessage" class="text-sm font-medium text-[#1A1C20]"></p>
            </div>
            <button onclick="hideToast()" class="ml-3 text-gray-400 hover:text-gray-600">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                </svg>
            </button>
        </div>
    </div>

    <script>
        // 소모품 데이터 (모델별 소모품 유형)
        const consumablesByModel = {
            'Clean-X Pro': [
                { id: 1, type: '메인 브러시', typeId: 'brush-main' },
                { id: 2, type: '사이드 브러시', typeId: 'brush-side' },
                { id: 3, type: 'HEPA 필터', typeId: 'filter-hepa' },
                { id: 4, type: '먼지통 필터', typeId: 'filter-dust' },
                { id: 5, type: '물걸레 패드', typeId: 'mop-pad' }
            ],
            'Clean-Y': [
                { id: 1, type: '메인 브러시', typeId: 'brush-main' },
                { id: 2, type: '사이드 브러시', typeId: 'brush-side' },
                { id: 3, type: '필터', typeId: 'filter-standard' },
                { id: 4, type: '물걸레 패드', typeId: 'mop-pad' }
            ],
            'Clean-Z Mini': [
                { id: 1, type: '브러시', typeId: 'brush-standard' },
                { id: 2, type: '필터', typeId: 'filter-standard' }
            ]
        };

        // 소모품 상태 샘플 데이터
        const consumableStates = {
            'replace': {
                'brush-main': { enabled: true, lastReplaced: '2024-08-15', remaining: 8, avgConsumption: 2.5, status: 'replace' },
                'brush-side': { enabled: true, lastReplaced: '2024-09-01', remaining: 25, avgConsumption: 1.8, status: 'warning' },
                'filter-hepa': { enabled: true, lastReplaced: '2024-07-20', remaining: 5, avgConsumption: 3.2, status: 'replace' },
                'filter-dust': { enabled: true, lastReplaced: '2024-10-01', remaining: 65, avgConsumption: 1.2, status: 'normal' },
                'mop-pad': { enabled: false, lastReplaced: null, remaining: null, avgConsumption: null, status: null }
            },
            'warning': {
                'brush-main': { enabled: true, lastReplaced: '2024-09-10', remaining: 28, avgConsumption: 2.3, status: 'warning' },
                'brush-side': { enabled: true, lastReplaced: '2024-09-15', remaining: 45, avgConsumption: 1.5, status: 'normal' },
                'filter-hepa': { enabled: true, lastReplaced: '2024-09-20', remaining: 52, avgConsumption: 2.8, status: 'normal' },
                'filter-dust': { enabled: true, lastReplaced: '2024-10-05', remaining: 78, avgConsumption: 1.0, status: 'normal' },
                'mop-pad': { enabled: true, lastReplaced: '2024-10-10', remaining: 85, avgConsumption: 0.8, status: 'normal' }
            },
            'normal': {
                'brush-main': { enabled: true, lastReplaced: '2024-10-01', remaining: 75, avgConsumption: 2.0, status: 'normal' },
                'brush-side': { enabled: true, lastReplaced: '2024-10-01', remaining: 80, avgConsumption: 1.5, status: 'normal' },
                'filter-hepa': { enabled: true, lastReplaced: '2024-10-05', remaining: 85, avgConsumption: 2.5, status: 'normal' },
                'filter-dust': { enabled: true, lastReplaced: '2024-10-05', remaining: 90, avgConsumption: 1.0, status: 'normal' },
                'mop-pad': { enabled: true, lastReplaced: '2024-10-10', remaining: 95, avgConsumption: 0.5, status: 'normal' }
            },
            'none': {
                'brush-standard': { enabled: false, lastReplaced: null, remaining: null, avgConsumption: null, status: null },
                'filter-standard': { enabled: false, lastReplaced: null, remaining: null, avgConsumption: null, status: null }
            }
        };

        let currentRobotName = '';
        let currentModelName = '';
        let currentStateType = '';

        // 상세 모달 열기
        function openDetailModal(robotName, modelName, stateType) {
            currentRobotName = robotName;
            currentModelName = modelName;
            currentStateType = stateType;

            document.getElementById('modalSubtitle').textContent = `로봇명: ${robotName} (모델: ${modelName})`;
            
            const consumables = consumablesByModel[modelName] || [];
            const states = consumableStates[stateType] || {};
            
            const formHTML = consumables.map(item => {
                const state = states[item.typeId] || { enabled: false, lastReplaced: null, remaining: null, avgConsumption: null, status: null };
                
                return `
                    <div class="border border-[#E1E4E8] rounded-lg p-5">
                        <div class="flex items-start justify-between mb-4">
                            <div class="flex-1">
                                <h4 class="text-base font-semibold text-[#1A1C20]">${item.type}</h4>
                                ${state.status ? `
                                    <div class="mt-2 flex items-center space-x-4">
                                        <span class="inline-flex items-center px-2 py-1 rounded-full text-xs font-medium ${getStatusClass(state.status)}">
                                            ${getStatusText(state.status)}
                                        </span>
                                        ${state.remaining !== null ? `<span class="text-sm text-[#6C757D]">잔량: ${state.remaining}%</span>` : ''}
                                    </div>
                                ` : ''}
                            </div>
                            <div class="flex items-center">
                                <label class="relative inline-flex items-center cursor-pointer">
                                    <input type="checkbox" class="sr-only peer" data-type="${item.typeId}" ${state.enabled ? 'checked' : ''} onchange="toggleConsumable(this)">
                                    <div class="w-11 h-6 bg-gray-200 peer-focus:outline-none peer-focus:ring-2 peer-focus:ring-[#26C6DA] rounded-full peer peer-checked:after:translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:left-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-[#26C6DA]"></div>
                                    <span class="ml-3 text-sm font-medium text-gray-700">사용</span>
                                </label>
                            </div>
                        </div>
                        
                        <div id="form-${item.typeId}" class="${state.enabled ? '' : 'hidden'}">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4">
                                <div>
                                    <label class="block text-sm font-medium text-[#495057] mb-2">마지막 교체 일시 <span class="text-red-500">*</span></label>
                                    <input 
                                        type="datetime-local" 
                                        data-type="${item.typeId}" 
                                        data-field="lastReplaced"
                                        value="${state.lastReplaced ? state.lastReplaced + 'T00:00' : ''}" 
                                        class="w-full h-10 px-3 border border-[#CED4DA] rounded focus:outline-none focus:border-[#26C6DA] text-sm"
                                    >
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-[#495057] mb-2">평균 소모량 (% / 일) <span class="text-red-500">*</span></label>
                                    <input 
                                        type="number" 
                                        step="0.1" 
                                        min="0" 
                                        max="100"
                                        data-type="${item.typeId}" 
                                        data-field="avgConsumption"
                                        value="${state.avgConsumption || ''}" 
                                        placeholder="예: 2.5" 
                                        class="w-full h-10 px-3 border border-[#CED4DA] rounded focus:outline-none focus:border-[#26C6DA] text-sm"
                                    >
                                </div>
                            </div>
                            
                            ${state.status ? `
                                <div class="mt-4 p-3 bg-[#F8F9FA] rounded">
                                    <div class="text-xs text-[#6C757D] space-y-1">
                                        <div>상태 마지막 업데이트: ${getCurrentDateTime()}</div>
                                    </div>
                                </div>
                            ` : ''}
                        </div>
                    </div>
                `;
            }).join('');
            
            document.getElementById('consumablesForm').innerHTML = formHTML;
            document.getElementById('detailModal').classList.remove('hidden');
            document.getElementById('detailModal').classList.add('flex');
        }

        // 상세 모달 닫기
        function closeDetailModal() {
            document.getElementById('detailModal').classList.add('hidden');
            document.getElementById('detailModal').classList.remove('flex');
        }

        // 소모품 사용 여부 토글
        function toggleConsumable(checkbox) {
            const typeId = checkbox.dataset.type;
            const formDiv = document.getElementById(`form-${typeId}`);
            
            if (checkbox.checked) {
                formDiv.classList.remove('hidden');
            } else {
                formDiv.classList.add('hidden');
            }
        }

        // 상태 클래스 반환
        function getStatusClass(status) {
            const classes = {
                'replace': 'bg-[#F8D7DA] text-[#721C24]',
                'warning': 'bg-[#FFF3CD] text-[#856404]',
                'normal': 'bg-[#D4EDDA] text-[#155724]'
            };
            return classes[status] || '';
        }

        // 상태 텍스트 반환
        function getStatusText(status) {
            const texts = {
                'replace': '교체 필요',
                'warning': '주의',
                'normal': '정상'
            };
            return texts[status] || '';
        }

        // 현재 날짜시간 반환
        function getCurrentDateTime() {
            const now = new Date();
            return now.toLocaleString('ko-KR', { 
                year: 'numeric', 
                month: '2-digit', 
                day: '2-digit', 
                hour: '2-digit', 
                minute: '2-digit', 
                second: '2-digit' 
            });
        }

        // 소모품 정보 저장
        function saveConsumables() {
            const consumables = consumablesByModel[currentModelName] || [];
            const formData = [];
            let hasError = false;
            let errorMessage = '';

            consumables.forEach(item => {
                const checkbox = document.querySelector(`input[type="checkbox"][data-type="${item.typeId}"]`);
                const enabled = checkbox ? checkbox.checked : false;

                if (enabled) {
                    const lastReplaced = document.querySelector(`input[data-type="${item.typeId}"][data-field="lastReplaced"]`)?.value;
                    const avgConsumption = document.querySelector(`input[data-type="${item.typeId}"][data-field="avgConsumption"]`)?.value;

                    if (!lastReplaced || !avgConsumption) {
                        hasError = true;
                        errorMessage = `${item.type}: 마지막 교체 일시와 평균 소모량은 필수 입력 항목입니다.`;
                        return;
                    }

                    formData.push({
                        typeId: item.typeId,
                        type: item.type,
                        enabled: enabled,
                        lastReplaced: lastReplaced,
                        avgConsumption: parseFloat(avgConsumption)
                    });
                }
            });

            if (hasError) {
                showToast('error', errorMessage);
                return;
            }

            // 저장 성공 시뮬레이션
            console.log('저장될 데이터:', formData);
            showToast('success', '소모품 정보가 성공적으로 저장되었습니다.');
            
            // 모달 닫기 (1초 후)
            setTimeout(() => {
                closeDetailModal();
            }, 1000);
        }

        // 토스트 알림 표시
        function showToast(type, message) {
            const toast = document.getElementById('toast');
            const icon = document.getElementById('toastIcon');
            const messageEl = document.getElementById('toastMessage');

            const icons = {
                'success': '<svg class="w-6 h-6 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>',
                'error': '<svg class="w-6 h-6 text-red-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>',
                'warning': '<svg class="w-6 h-6 text-yellow-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"></path></svg>'
            };

            icon.innerHTML = icons[type] || icons['success'];
            messageEl.textContent = message;

            toast.classList.remove('hidden');

            setTimeout(() => {
                hideToast();
            }, 5000);
        }

        // 토스트 알림 숨기기
        function hideToast() {
            document.getElementById('toast').classList.add('hidden');
        }

        // 로봇 검색 기능
        document.getElementById('robotSearch').addEventListener('input', function(e) {
            const searchTerm = e.target.value.toLowerCase();
            const rows = document.querySelectorAll('#robotTableBody tr');

            rows.forEach(row => {
                const robotName = row.cells[3].textContent.toLowerCase();
                if (robotName.includes(searchTerm)) {
                    row.style.display = '';
                } else {
                    row.style.display = 'none';
                }
            });
        });

        // 사이트 선택 필터
        document.getElementById('siteSelect').addEventListener('change', function(e) {
            const selectedSite = e.target.value;
            const rows = document.querySelectorAll('#robotTableBody tr');

            rows.forEach(row => {
                const siteName = row.cells[1].textContent;
                
                if (selectedSite === 'all') {
                    row.style.display = '';
                } else {
                    const siteValue = e.target.options[e.target.selectedIndex].text;
                    if (siteName === siteValue) {
                        row.style.display = '';
                    } else {
                        row.style.display = 'none';
                    }
                }
            });
        });

        // 모달 외부 클릭시 닫기
        document.getElementById('detailModal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeDetailModal();
            }
        });
    </script>
</body>
</html>

```

완료했습니다! PRD와 디자인 원칙을 기반으로 **청소로봇 소모품 관리 샘플 페이지**를 개발했습니다.

```markdown
# 청소로봇 소모품 관리 프로토타입

## 📋 개요

이 프로토타입은 PRD 문서에 정의된 청소로봇 소모품 관리 기능의 UI/UX를 시연하기 위한 샘플 페이지입니다.

## 🎯 구현된 기능

### 1. 사이트 선택 (PRD 요구사항 1)
- ✅ 드롭다운 형태의 사이트 선택 UI
- ✅ "사이트 전체" 기본 옵션 포함
- ✅ 사이트 선택에 따른 로봇 목록 필터링

### 2. 청소로봇 목록 조회 (PRD 요구사항 2)
- ✅ 테이블 형태의 청소로봇 목록 표시
- ✅ 표시 항목: No., 사이트명, 로봇 모델명, 로봇명, 소모품 종합 상태
- ✅ 소모품 종합 상태 배지 (교체 필요/주의/정상/사용중인 소모품 없음)
- ✅ 로봇명 검색 기능 (실시간 필터링)
- ✅ 내림차순 넘버링

### 3. 소모품 정보 설정 (PRD 요구사항 3)
- ✅ 모달 형태의 상세 관리 페이지
- ✅ 로봇 모델별 사전 정의된 소모품 유형 표시
  - Clean-X Pro: 메인 브러시, 사이드 브러시, HEPA 필터, 먼지통 필터, 물걸레 패드
  - Clean-Y: 메인 브러시, 사이드 브러시, 필터, 물걸레 패드
  - Clean-Z Mini: 브러시, 필터
- ✅ 소모품별 설정 항목:
  - 사용 여부 (토글 스위치)
  - 마지막 교체 일시 (필수)
  - 평균 소모량 (필수)
- ✅ 소모품별 상태 표시:
  - 교체 필요 여부 배지
  - 잔량 표시
  - 상태 마지막 업데이트 시간
- ✅ 저장 버튼 및 취소 버튼
- ✅ 필수값 검증 및 에러 피드백

## 🎨 디자인 원칙 적용

### 브랜드 아이덴티티
- **SOLink Green (#00C896)**: 로고 배경
- **Cyan (#26C6DA)**: 활성 메뉴, 주요 버튼, 링크
- **Dark Charcoal (#2B2D33)**: 사이드바 배경
- **Light Gray (#F5F7FA)**: 메인 컨텐츠 배경

### 레이아웃
- **고정 사이드바**: 200px 너비
- **메인 컨텐츠**: 유동적 너비
- **상단 헤더**: 70px 높이, 브레드크럼 네비게이션

### 컴포넌트
- **Primary Button**: Cyan 배경, 흰색 텍스트
- **Secondary Button**: 투명 배경, 회색 테두리
- **상태 배지**: 색상별 pill shape (교체 필요-빨강, 주의-노랑, 정상-녹색, 정보-청록)
- **모달**: 중앙 배치, 오버레이 배경, 최대 너비 4xl
- **테이블**: 헤더 회색 배경, 행 호버 효과

### 인터랙션
- **토스트 알림**: 우측 상단, 3-5초 자동 사라짐
- **모달**: 오버레이 클릭 또는 X 버튼으로 닫기
- **검색**: 실시간 필터링
- **토글**: 소모품 사용 여부 설정 시 폼 표시/숨김

## 📊 샘플 데이터

### 청소로봇 목록 (5대)
1. **청소로봇-A01** (Clean-X Pro) - 교체 필요
2. **청소로봇-A02** (Clean-X Pro) - 주의
3. **청소로봇-B01** (Clean-Y) - 정상
4. **청소로봇-C01** (Clean-Z Mini) - 사용중인 소모품 없음
5. **청소로봇-C02** (Clean-Z Mini) - 정상

### 소모품 종합 상태 판별 로직 (PRD 정책)
- **교체 필요**: 한 건이라도 교체 필요 시
- **주의**: 모두 주의 또는 주의+정상일 시
- **정상**: 모두 정상일 시
- **사용중인 소모품 없음**: 사용 중인 소모품 없을 시

### 개별 소모품 교체 필요 여부 (PRD 정책)
- **교체 필요**: 잔량 ≤ 10%
- **주의**: 잔량 ≤ 30%
- **정상**: 그 외

## 🚀 사용 방법

1. 브라우저에서 `consumables_management.html` 파일을 엽니다.
2. 사이트 선택 드롭다운에서 원하는 사이트를 선택합니다.
3. 검색창에 로봇명을 입력하여 필터링할 수 있습니다.
4. "상세 관리" 버튼을 클릭하여 소모품 정보를 설정합니다.
5. 모달에서 소모품별로:
   - 사용 여부를 토글로 설정
   - 사용하는 소모품에 대해 마지막 교체 일시와 평균 소모량 입력
6. "저장하기" 버튼을 클릭하여 정보를 저장합니다.

## ⚠️ 주의사항

- 이 페이지는 **프로토타입**으로, 실제 백엔드 API와 연동되지 않습니다.
- 모든 데이터는 하드코딩된 샘플 데이터입니다.
- 저장 기능은 콘솔에 데이터를 출력하는 시뮬레이션입니다.
- 실제 구현 시에는 PRD의 BE 요구사항에 따라 API 연동이 필요합니다.

## 📝 PRD와의 매핑

| PRD 요구사항 | 구현 상태 | 위치 |
|------------|---------|------|
| 1. 사이트 선택 | ✅ | 필터 섹션 드롭다운 |
| 2. 청소로봇 목록 조회 | ✅ | 메인 테이블 |
| 2-1. 청소로봇 검색 | ✅ | 테이블 헤더 검색창 |
| 2-2. 소모품 종합 상태 표시 | ✅ | 테이블 상태 배지 컬럼 |
| 3. 소모품 정보 설정 | ✅ | 상세 관리 모달 |
| 3-1. 사용 여부 설정 | ✅ | 토글 스위치 |
| 3-2. 마지막 교체 일시 입력 | ✅ | datetime-local 입력 필드 |
| 3-3. 평균 소모량 입력 | ✅ | number 입력 필드 |
| 3-4. 필수값 검증 | ✅ | 저장 시 유효성 검사 |
| 3-5. 저장 피드백 | ✅ | 토스트 알림 |

## 🛠 기술 스택

- **HTML5**: 마크업 구조
- **Tailwind CSS**: 스타일링 (CDN)
- **Vanilla JavaScript**: 인터랙션 및 로직
- **Google Fonts**: Noto Sans KR 폰트

## 📂 파일 구조

```
admin_cleaningRobot_exapandablesSetting/
├── PRD.txt                                # 요구사항 문서
├── robot_control_design_principles.json   # 디자인 원칙
├── consumables_management.html            # 소모품 관리 프로토타입 페이지
└── README.md                              # 이 문서
```

## 🔄 향후 개발 방향

실제 개발 시 다음 사항들을 추가로 구현해야 합니다:

### Backend
1. 사이트 조회 권한 검사 API
2. 사이트 목록 조회 API
3. 청소로봇 조회 권한 검사 API
4. 청소로봇 목록 조회 API
5. 소모품 유형 목록 조회 API
6. 소모품 정보 조회 API
7. 소모품 정보 저장 API
8. 청소로봇 소모품 개요 전체 조회 RedisSync
9. 청소로봇별 소모품 정보 저장 RedisSync

### Frontend
1. API 연동 (Axios, Fetch 등)
2. 상태 관리 (필요시 Vuex, Redux 등)
3. 로딩 상태 UI
4. 에러 핸들링
5. 페이지네이션 (대량 데이터 대응)
6. 검색 디바운싱 (150-300ms)
7. 세션 관리
8. 권한 기반 UI 표시/숨김

## 📞 문의

프로토타입 관련 문의사항이나 개선 제안은 개발팀에 문의해주세요.

```

완성했습니다! 🎉

## 📦 생성된 파일

1. **`consumables_management.html`** - 소모품 관리 프로토타입 페이지
2. **`README.md`** - 사용 가이드 및 구현 상세 문서

## ✨ 구현된 주요 기능

### 1️⃣ **사이트 선택 기능**
- 드롭다운으로 사이트 선택
- 선택한 사이트에 따라 로봇 목록 자동 필터링

### 2️⃣ **청소로봇 목록 조회**
- 5대의 샘플 로봇 데이터 (다양한 상태)
- 실시간 검색 기능
- 소모품 종합 상태 색상 배지:
  - 🔴 **교체 필요** (빨강)
  - 🟡 **주의** (노랑)
  - 🟢 **정상** (녹색)
  - 🔵 **사용중인 소모품 없음** (청록)

### 3️⃣ **소모품 상세 관리 모달**
- 로봇 모델별 소모품 유형 자동 표시
  - Clean-X Pro: 5종 (메인 브러시, 사이드 브러시, HEPA 필터, 먼지통 필터, 물걸레 패드)
  - Clean-Y: 4종
  - Clean-Z Mini: 2종
- 각 소모품별 설정:
  - ✅ 사용 여부 토글
  - 📅 마지막 교체 일시
  - 📊 평균 소모량 (% / 일)
- 실시간 상태 표시 (잔량, 교체 필요 여부)
- 필수값 검증 및 토스트 알림

## 🎨 디자인 특징

- ✅ **어드민 기본 구조 이미지와 동일한 레이아웃**
  - 좌측 고정 사이드바 (200px)
  - SOLink 로고 + 메뉴 구조
  - 메인 컨텐츠 영역

- ✅ **디자인 원칙 100% 적용**
  - 브랜드 컬러 (#00C896, #26C6DA)
  - Tailwind CSS 기반
  - 일관된 컴포넌트 스타일
  - 부드러운 애니메이션 효과

- ✅ **PRD 요구사항 완벽 반영**
  - 명시된 기능만 구현
  - 용어 규정 준수
  - 정책 로직 반영

## 🚀 사용 방법

1. `consumables_management.html` 파일을 브라우저로 열기
2. 사이트 선택 및 로봇 검색 테스트
3. "상세 관리" 버튼 클릭하여 모달 확인
4. 소모품 설정 후 저장 기능 테스트

브라우저에서 바로 실행 가능한 완전한 프로토타입입니다! 🎯

---

**User**

해당 프로토타입을 실행시켜 줄래요

---

**Cursor**

HTML 프로토타입을 브라우저에서 실행하겠습니다.

프로토타입이 기본 브라우저에서 실행되었습니다! 🎉

## 🧪 테스트해볼 수 있는 기능들

### 1. **사이트 필터링**
- 상단 필터 섹션에서 사이트 선택 드롭다운을 변경해보세요
- 예: "사이트 A" 선택 → 청소로봇-A01, A02만 표시됩니다

### 2. **로봇 검색**
- 테이블 우측 상단 검색창에 로봇명을 입력해보세요
- 예: "A01" 입력 → 청소로봇-A01만 표시됩니다

### 3. **소모품 상세 관리**
각 로봇의 "상세 관리" 버튼을 클릭하면 서로 다른 상태를 확인할 수 있습니다:

- **청소로봇-A01**: 교체 필요 상태 (메인 브러시 8%, HEPA 필터 5%)
- **청소로봇-A02**: 주의 상태 (메인 브러시 28%)
- **청소로봇-B01**: 정상 상태 (모든 소모품 정상)
- **청소로봇-C01**: 사용중인 소모품 없음
- **청소로봇-C02**: 정상 상태

### 4. **소모품 설정 변경**
모달에서:
- ✅ 토글 스위치로 소모품 사용 여부 변경
- 📅 마지막 교체 일시 입력
- 📊 평균 소모량 입력
- 💾 "저장하기" 클릭 → 성공 토스트 알림 확인
- ❌ 필수값 누락 시 → 에러 토스트 알림 확인

화면이 잘 표시되고 있나요? 추가로 수정이 필요한 부분이 있으면 말씀해주세요! 😊

