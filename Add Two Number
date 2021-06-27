/// Link for Question :    https://leetcode.com/problems/add-two-numbers/submissions/

/// #Add_two_numbers  #Leetcode #javaSolution

/// Solution

/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {
    public ListNode addTwoNumbers(ListNode l1, ListNode l2) {
        
        ListNode tra = new ListNode();
        ListNode res = tra;
        int carry = 0;
        while(l1 != null && l2 != null){
            int temp = l1.val + l2.val + carry;
             ListNode node;
            if(temp > 9)
             node = new ListNode(temp % 10);
            else
                node = new ListNode(temp);
            tra.next = node;
            tra = tra.next;
            carry = temp /10;
            l1 = l1.next;
            l2 = l2.next;
        }
        
        while(l1 != null){
            int temp = l1.val + carry;
             ListNode node;
            if(temp > 9)
             node = new ListNode(temp % 10);
            else
                node = new ListNode(temp);
        
            tra.next = node;
            tra = tra.next;
            carry = temp /10;
            l1 = l1.next;
            
        }
         while(l2 != null){
            int temp = l2.val + carry;
             ListNode node;
            if(temp > 9)
             node = new ListNode(temp % 10);
            else
                node = new ListNode(temp);
        
            tra.next = node;
            tra = tra.next;
            carry = temp /10;
            l2 = l2.next;
            
        }
        
        while(carry > 0){
            
             ListNode node;
        
             node = new ListNode(carry);
            carry = carry /10;
            tra.next = node;
            tra = tra.next;
        
            
        }
        
        return res.next;
    }
}
