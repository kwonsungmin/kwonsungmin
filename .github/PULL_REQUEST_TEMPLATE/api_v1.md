# 📋 API Pull Request

## 📌 Description
<!-- 이 PR이 어떤 변경 사항을 포함하는지 간략히 설명하세요. -->
- 변경된 API의 주요 내용
- 새로운 API 추가 또는 기존 API 수정 여부
- 관련된 이슈 또는 작업 요청 (예: Jira Issue Key)

---

## 🔗 Related Issues
<!-- 관련된 이슈를 연결하거나 링크를 추가하세요. -->
- Resolves: #[이슈 번호]
- Related to: #[이슈 번호]

---

## 🚀 Changes
<!-- 변경된 API의 주요 내용을 작성하세요. -->
- [ ] 새로운 API 추가
  - **엔드포인트**: `[GET/POST/PUT/DELETE] /api/v1/resource`
  - **요청(Request) 데이터**:
    ```json
    {
      "key": "value"
    }
    ```
  - **응답(Response) 데이터**:
    ```json
    {
      "status": "success",
      "data": { "id": 1 }
    }
    ```
- [ ] 기존 API 수정
  - **변경된 엔드포인트**: `[GET] /api/v1/resource`
  - **변경 사항**: 
    - 요청 필드 추가: `key: string`
    - 응답 데이터 구조 변경

---

## ✅ Checklist
<!-- PR의 준비 상태를 확인하기 위한 체크리스트 -->
- [ ] 코드 변경 사항이 정상적으로 동작함을 확인했습니다.
- [ ] Unit Test 작성 또는 수정했습니다.
- [ ] Integration Test 작성 또는 수정했습니다.
- [ ] Swagger/Redoc 문서를 업데이트했습니다.
- [ ] API 요청/응답 데이터에 대한 Validation을 검토했습니다.
- [ ] 에러 핸들링 로직을 추가 또는 검토했습니다.
- [ ] 기존 API와의 호환성을 확인했습니다.

---

## 🛠️ How to Test
<!-- 이 변경 사항을 테스트하는 방법을 작성하세요. -->
1. **API 요청**:
   - Method: `[GET/POST/PUT/DELETE]`
   - URL: `http://localhost:3000/api/v1/resource`
   - Request Body (필요한 경우):
     ```json
     {
       "key": "value"
     }
     ```
2. **테스트 시나리오**:
   - 정상 요청 시 200 응답 확인
   - 유효하지 않은 입력값에 대해 적절한 에러 응답 확인
   - 각 시나리오별 Integration Test 수행

---

## 🖼️ Screenshots or Logs (Optional)
<!-- API 요청/응답 또는 로깅 정보를 첨부하세요 (선택 사항) -->
| **Request**            | **Response**                |
|-------------------------|-----------------------------|
| `GET /api/v1/resource` | `{ "status": "success" }`   |

---

## 📄 Additional Comments
<!-- 추가적으로 논의해야 할 사항이나 배포에 필요한 정보를 작성하세요. -->
- 배포 후 클라이언트에 영향을 미칠 가능성이 있는 변경 사항
- 성능 관련 고려 사항 또는 추후 개선 사항
