//# Java
//记录学习路上的绊脚石
package com.yang.java;

public class ArrayTest01 {
	public static void main(String[] args) {
		int[] arr = new int[10];
		int area = 0,count = 0;
		for (int i = 0; i < arr.length; i++) {
			arr[i] = (int)(Math.random()*90 + 10);
//			System.out.println(arr[i]);
		}
		//最大值
		int maxValue = arr[0];
		for (int j = 0; j < arr.length; j++) {
			if(maxValue < arr[j]) {
				maxValue = arr[j];
			}
		}
		//最小值
		int minValue = arr[0];
		for (int k = 0; k < arr.length; k++) {
			if(minValue > arr[k]) {
				minValue = arr[k];
			}
		}
		
		for (int h = 0; h < arr.length; h++) {
			count += arr[h];
			area = count/arr.length;
		}

			
		System.out.println("最大值："+maxValue+"最小值："+minValue+"平均值："+area+"和："+ count);
	}
}
