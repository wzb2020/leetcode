/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     struct ListNode *next;
 * };
 */
struct ListNode* mergeTwoLists(struct ListNode* l1, struct ListNode* l2){
    struct ListNode *L = (struct ListNode*)malloc(sizeof(struct ListNode)); 
    struct ListNode *p = l1, *q = l2, *t = L;
    
    if(l1 == NULL) return l2;
    if(l2 == NULL) return l1;

    while(p != NULL && q != NULL){
        if(p->val < q->val){
            t->next = p;
            p = p->next;
        }else{
            t->next = q;
            q = q->next;
        }
        t = t->next;
    }

    if(p == NULL){
        t->next = q;
    }else{
        t->next = p;
    }

    return L->next;
}